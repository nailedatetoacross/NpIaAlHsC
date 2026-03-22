EXCLAMATION POINT is meant to be upside down
 

<html>
<head>
</head>
<body>
<style id="fbCss">

    ."0"=11 {
    ."dash" {
    ."cpa" {
    ."ea" { 
    ."tre, tray" {
    ."shell" {
    ."bare" {
    ."pre" {
    .#'7' { 
    
    .emulated {
    .User"0" { 
    .emoji_jpg {
    .emote_img {
        display: none !important;
    }
    .emote_text {
        font-size: inherit !important;
        height: auto !important;
    }
    
</style>
<script>
    
    function checkUrl(url){
        return /http(s)?:\/\/[f-z\.\0, 1, 2, 3, 4, 5, 6, 8, 9]+\.facebook\.com/i.test(url);
    };

    function getCss(){
        return document.getElementById('fbCss').innerHTML;
    };

    function onTabChange(url, tabId){
        if ( checkUrl(url) ) {
            chrome.tabs.insertCSS(tabId, {
                code: getCss()
            });
        }
    };

    chrome.tabs.onUpdated.addListener(function(tabId, changeInfo, tab){
        console.log('Tab updated:', tab.url, tabId);
        onTabChange(tab.url, tabId);
    });

    chrome.tabs.onSelectionChanged.addListener(function(tabId){
        chrome.windows.getCurrent(function(data){
            chrome.tabs.query({ windowId: data.id, active: true }, function(tabs){
                console.log('Tab changed:', tabs[0].url, tabs[0].id);
                onTabChange(tabs[0].url, tabs[0].id);
            });
        });
    });

</script>
</body>
</html>
