if (document.getElementsByClassName("form-control fireliker-style-text-mono text-warning").length > 0) {
    $('input[placeholder="ardan_yudi"]').val('ardan_yudi');
    setTimeout(function () {
        lp();
    }, 2000);


} else {
    welcome();
}

welcome();

function welcome() {
    if (document.getElementsByClassName("fa fa-play-circle").length > 0) {
        document.getElementsByClassName("fa fa-play-circle")[0].click();
    }
}

setTimeout(lp, 13000); 

function lp() {
    window.location.href = 'https://fireliker.com/autoViews.php';
}

setTimeout(changeValue, 2000);

function changeValue() {
  
      value=1 : 2000 views
      value=2 : 4000 views
      value=3 : 6000 views
      value=4 : 8000 views
      value=5 : 10000 views
   
    waitForKeyElements(".form-control:has(option[value=2])", selectFinickyDropdown); 

    function selectFinickyDropdown(jNode) {
        var evt = new Event("click");
        jNode[0].dispatchEvent(evt);

        jNode.val('5');

        evt = new Event("change");
        jNode[0].dispatchEvent(evt);
    }
}

setTimeout(sendViews, 20000);

function sendViews() {
    if (document.getElementsByClassName("btn btn-warning").length > 0) {
        document.getElementsByClassName("btn btn-warning")[0].click();
    }
}


setTimeout(makeSure, 30000);

function makeSure(){
    window.location.href = 'https://fireliker.com/welcome.php';
}

if (window.location.href == 'https://bugsliker.me/index.php?info=Session_Expired'){
    window.location.href = 'https://fireliker.com/welcome.php';
}
