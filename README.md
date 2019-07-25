# demo_quiz

file : script_souce.js

/*
document.onselectstart = function () {

    alert("This function is disabled!");
    
    return false;
    
};
*/

//above is replaced by the code below

   function killCopy(e){
        return false
    }
    
    function reEnable(){
        return true
    }
    
    document.onselectstart=new Function ("return false")
    
    if (window.sidebar){
        document.onmousedown=killCopy
        document.onclick=reEnable
    }
