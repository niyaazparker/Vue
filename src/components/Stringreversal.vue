

    <template>
        <div>
            <h1>String reversal</h1>
            
                <input class="form-control" v-model="inputStr" @input="reverseString" placeholder="Enter a string">
                <p>Reversed String: {{ reversedStr }}</p>
               
        </div>
    </template>

    <script>
    export default {
    name: 'StringReversal',
    data() {
        return {
            inputStr: '',
            reversedStr: ''
        };
    },
    methods: {
        reverseString() {
            this.reversedStr = this.inputStr.split('').reverse().join('');
        }
    }
};
</script>

