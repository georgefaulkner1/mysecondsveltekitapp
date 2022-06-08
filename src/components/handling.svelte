<script>
    function Handler(data){
        let res = {}
        if(data.data) res.data = data.data
        if(data.status) res.statusCode = data.status
        return res
    }
</script>