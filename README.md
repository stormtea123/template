Template
=====

模板引擎初探...

    var template = "我喜欢{{what}}";
    var data = {
        "what":"美女"
    }
    var result = template.replace(/{{(\w+)}}/g,function(a,b){
        return data[b];
    })
    console.log(result)

……