
    <template>
        <div>
            <h1>Library Books</h1>
            <div class="d-flex mx-auto mb-3">
                <!-- Search input -->
                <input class="form-control" type="text" v-model="searchTerm" placeholder="Search by title or author">

                <!-- Sort buttons -->
                <button class="btn btn-primary mx-1 btn-sm" @click="toggleSort('title')">Title ({{ sortBy === 'title' ? sortOrder : 'asc' }})</button>
                <button class="btn btn-primary mx-1 btn-sm" @click="toggleSort('author')">Author ({{ sortBy === 'author' ? sortOrder : 'asc' }})</button>
            </div>
            <!-- Book list -->
                <ul>
                    <li class="text-start" v-for="book in filteredBooks" :key="book.title">
                        {{ book.title }} by {{ book.author }} ({{ book.year }})
                    </li>
                </ul>
        </div>
    </template>
<script>
export default {
    name: 'LibraryBooks',
    data() {
        return {
            searchTerm: '',
            sortBy: 'title',
            sortOrder: 'asc',
            books: [
                { title: 'The Great Gatsby', author: 'F. Scott Fitzgerald', year: 1925 },
                { title: 'To Kill a Mockingbird', author: 'Harper Lee', year: 1960 },
                // Add more books as needed
            ]
        };
    },
    computed: {
        filteredBooks() {
            const searchTerm = this.searchTerm.toLowerCase();
            return this.books.filter(book => {
                const titleMatch = book.title.toLowerCase().includes(searchTerm);
                const authorMatch = book.author.toLowerCase().includes(searchTerm);
                return titleMatch || authorMatch;
            }).sort((a, b) => {
                const order = this.sortOrder === 'asc' ? 1 : -1;
                return a[this.sortBy].localeCompare(b[this.sortBy]) * order;
            });
        }
    },

methods: {
        toggleSort(key) {
            if (this.sortBy === key) {
                // If already sorting by the same key, toggle the sort order
                this.sortOrder = this.sortOrder === 'asc' ? 'desc' : 'asc';
            } else {
                // If sorting by a new key, set the key and default to ascending order
                this.sortBy = key;
                this.sortOrder = 'asc';
            }
        }
    }
};
</script>

