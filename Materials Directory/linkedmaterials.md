










    


<!DOCTYPE html>
<html lang="en" class="sticky-footer" >
    <head>
        
    <title>SurveyMonkey Survey Summary - Parent Survey</title>


        <meta charset="utf-8"><script type="text/javascript">(window.NREUM||(NREUM={})).loader_config={xpid:"UwUPVVJXGwcDVFJVBQM="};window.NREUM||(NREUM={}),__nr_require=function(t,e,n){function r(n){if(!e[n]){var o=e[n]={exports:{}};t[n][0].call(o.exports,function(e){var o=t[n][1][e];return r(o||e)},o,o.exports)}return e[n].exports}if("function"==typeof __nr_require)return __nr_require;for(var o=0;o<n.length;o++)r(n[o]);return r}({1:[function(t,e,n){function r(t){try{s.console&&console.log(t)}catch(e){}}var o,i=t("ee"),a=t(14),s={};try{o=localStorage.getItem("__nr_flags").split(","),console&&"function"==typeof console.log&&(s.console=!0,-1!==o.indexOf("dev")&&(s.dev=!0),-1!==o.indexOf("nr_dev")&&(s.nrDev=!0))}catch(c){}s.nrDev&&i.on("internal-error",function(t){r(t.stack)}),s.dev&&i.on("fn-err",function(t,e,n){r(n.stack)}),s.dev&&(r("NR AGENT IN DEVELOPMENT MODE"),r("flags: "+a(s,function(t,e){return t}).join(", ")))},{}],2:[function(t,e,n){function r(t,e,n,r,o){try{d?d-=1:i("err",[o||new UncaughtException(t,e,n)])}catch(s){try{i("ierr",[s,(new Date).getTime(),!0])}catch(c){}}return"function"==typeof f?f.apply(this,a(arguments)):!1}function UncaughtException(t,e,n){this.message=t||"Uncaught error with no additional information",this.sourceURL=e,this.line=n}function o(t){i("err",[t,(new Date).getTime()])}var i=t("handle"),a=t(15),s=t("ee"),c=t("loader"),f=window.onerror,u=!1,d=0;c.features.err=!0,t(1),window.onerror=r;try{throw new Error}catch(l){"stack"in l&&(t(8),t(7),"addEventListener"in window&&t(5),c.xhrWrappable&&t(9),u=!0)}s.on("fn-start",function(t,e,n){u&&(d+=1)}),s.on("fn-err",function(t,e,n){u&&(this.thrown=!0,o(n))}),s.on("fn-end",function(){u&&!this.thrown&&d>0&&(d-=1)}),s.on("internal-error",function(t){i("ierr",[t,(new Date).getTime(),!0])})},{}],3:[function(t,e,n){t("loader").features.ins=!0},{}],4:[function(t,e,n){function r(t){}if(window.performance&&window.performance.timing&&window.performance.getEntriesByType){var o=t("ee"),i=t("handle"),a=t(8),s=t(7);t("loader").features.stn=!0,t(6);var c=NREUM.o.EV;o.on("fn-start",function(t,e){var n=t[0];n instanceof c&&(this.bstStart=Date.now())}),o.on("fn-end",function(t,e){var n=t[0];n instanceof c&&i("bst",[n,e,this.bstStart,Date.now()])}),a.on("fn-start",function(t,e,n){this.bstStart=Date.now(),this.bstType=n}),a.on("fn-end",function(t,e){i("bstTimer",[e,this.bstStart,Date.now(),this.bstType])}),s.on("fn-start",function(){this.bstStart=Date.now()}),s.on("fn-end",function(t,e){i("bstTimer",[e,this.bstStart,Date.now(),"requestAnimationFrame"])}),o.on("pushState-start",function(t){this.time=Date.now(),this.startPath=location.pathname+location.hash}),o.on("pushState-end",function(t){i("bstHist",[location.pathname+location.hash,this.startPath,this.time])}),"addEventListener"in window.performance&&(window.performance.clearResourceTimings?window.performance.addEventListener("resourcetimingbufferfull",function(t){i("bstResource",[window.performance.getEntriesByType("resource")]),window.performance.clearResourceTimings()},!1):window.performance.addEventListener("webkitresourcetimingbufferfull",function(t){i("bstResource",[window.performance.getEntriesByType("resource")]),window.performance.webkitClearResourceTimings()},!1)),document.addEventListener("scroll",r,!1),document.addEventListener("keypress",r,!1),document.addEventListener("click",r,!1)}},{}],5:[function(t,e,n){function r(t){for(var e=t;e&&!e.hasOwnProperty(u);)e=Object.getPrototypeOf(e);e&&o(e)}function o(t){s.inPlace(t,[u,d],"-",i)}function i(t,e){return t[1]}var a=t("ee").get("events"),s=t(16)(a),c=t("gos"),f=XMLHttpRequest,u="addEventListener",d="removeEventListener";e.exports=a,"getPrototypeOf"in Object?(r(document),r(window),r(f.prototype)):f.prototype.hasOwnProperty(u)&&(o(window),o(f.prototype)),a.on(u+"-start",function(t,e){if(t[1]){var n=t[1];if("function"==typeof n){var r=c(n,"nr@wrapped",function(){return s(n,"fn-",null,n.name||"anonymous")});this.wrapped=t[1]=r}else"function"==typeof n.handleEvent&&s.inPlace(n,["handleEvent"],"fn-")}}),a.on(d+"-start",function(t){var e=this.wrapped;e&&(t[1]=e)})},{}],6:[function(t,e,n){var r=t("ee").get("history"),o=t(16)(r);e.exports=r,o.inPlace(window.history,["pushState","replaceState"],"-")},{}],7:[function(t,e,n){var r=t("ee").get("raf"),o=t(16)(r);e.exports=r,o.inPlace(window,["requestAnimationFrame","mozRequestAnimationFrame","webkitRequestAnimationFrame","msRequestAnimationFrame"],"raf-"),r.on("raf-start",function(t){t[0]=o(t[0],"fn-")})},{}],8:[function(t,e,n){function r(t,e,n){t[0]=a(t[0],"fn-",null,n)}function o(t,e,n){this.method=n,this.timerDuration="number"==typeof t[1]?t[1]:0,t[0]=a(t[0],"fn-",this,n)}var i=t("ee").get("timer"),a=t(16)(i);e.exports=i,a.inPlace(window,["setTimeout","setImmediate"],"setTimer-"),a.inPlace(window,["setInterval"],"setInterval-"),a.inPlace(window,["clearTimeout","clearImmediate"],"clearTimeout-"),i.on("setInterval-start",r),i.on("setTimer-start",o)},{}],9:[function(t,e,n){function r(t,e){d.inPlace(e,["onreadystatechange"],"fn-",s)}function o(){var t=this,e=u.context(t);t.readyState>3&&!e.resolved&&(e.resolved=!0,u.emit("xhr-resolved",[],t)),d.inPlace(t,v,"fn-",s)}function i(t){w.push(t),h&&(g=-g,b.data=g)}function a(){for(var t=0;t<w.length;t++)r([],w[t]);w.length&&(w=[])}function s(t,e){return e}function c(t,e){for(var n in t)e[n]=t[n];return e}t(5);var f=t("ee"),u=f.get("xhr"),d=t(16)(u),l=NREUM.o,p=l.XHR,h=l.MO,m="readystatechange",v=["onload","onerror","onabort","onloadstart","onloadend","onprogress","ontimeout"],w=[];e.exports=u;var y=window.XMLHttpRequest=function(t){var e=new p(t);try{u.emit("new-xhr",[e],e),e.addEventListener(m,o,!1)}catch(n){try{u.emit("internal-error",[n])}catch(r){}}return e};if(c(p,y),y.prototype=p.prototype,d.inPlace(y.prototype,["open","send"],"-xhr-",s),u.on("send-xhr-start",function(t,e){r(t,e),i(e)}),u.on("open-xhr-start",r),h){var g=1,b=document.createTextNode(g);new h(a).observe(b,{characterData:!0})}else f.on("fn-end",function(t){t[0]&&t[0].type===m||a()})},{}],10:[function(t,e,n){function r(t){var e=this.params,n=this.metrics;if(!this.ended){this.ended=!0;for(var r=0;l>r;r++)t.removeEventListener(d[r],this.listener,!1);if(!e.aborted){if(n.duration=(new Date).getTime()-this.startTime,4===t.readyState){e.status=t.status;var i=o(t,this.lastSize);if(i&&(n.rxSize=i),this.sameOrigin){var a=t.getResponseHeader("X-NewRelic-App-Data");a&&(e.cat=a.split(", ").pop())}}else e.status=0;n.cbTime=this.cbTime,u.emit("xhr-done",[t],t),c("xhr",[e,n,this.startTime])}}}function o(t,e){var n=t.responseType;if("json"===n&&null!==e)return e;var r="arraybuffer"===n||"blob"===n||"json"===n?t.response:t.responseText;return i(r)}function i(t){if("string"==typeof t&&t.length)return t.length;if("object"==typeof t){if("undefined"!=typeof ArrayBuffer&&t instanceof ArrayBuffer&&t.byteLength)return t.byteLength;if("undefined"!=typeof Blob&&t instanceof Blob&&t.size)return t.size;if(!("undefined"!=typeof FormData&&t instanceof FormData))try{return JSON.stringify(t).length}catch(e){return}}}function a(t,e){var n=f(e),r=t.params;r.host=n.hostname+":"+n.port,r.pathname=n.pathname,t.sameOrigin=n.sameOrigin}var s=t("loader");if(s.xhrWrappable){var c=t("handle"),f=t(11),u=t("ee"),d=["load","error","abort","timeout"],l=d.length,p=t("id"),h=t(13),m=window.XMLHttpRequest;s.features.xhr=!0,t(9),u.on("new-xhr",function(t){var e=this;e.totalCbs=0,e.called=0,e.cbTime=0,e.end=r,e.ended=!1,e.xhrGuids={},e.lastSize=null,h&&(h>34||10>h)||window.opera||t.addEventListener("progress",function(t){e.lastSize=t.loaded},!1)}),u.on("open-xhr-start",function(t){this.params={method:t[0]},a(this,t[1]),this.metrics={}}),u.on("open-xhr-end",function(t,e){"loader_config"in NREUM&&"xpid"in NREUM.loader_config&&this.sameOrigin&&e.setRequestHeader("X-NewRelic-ID",NREUM.loader_config.xpid)}),u.on("send-xhr-start",function(t,e){var n=this.metrics,r=t[0],o=this;if(n&&r){var a=i(r);a&&(n.txSize=a)}this.startTime=(new Date).getTime(),this.listener=function(t){try{"abort"===t.type&&(o.params.aborted=!0),("load"!==t.type||o.called===o.totalCbs&&(o.onloadCalled||"function"!=typeof e.onload))&&o.end(e)}catch(n){try{u.emit("internal-error",[n])}catch(r){}}};for(var s=0;l>s;s++)e.addEventListener(d[s],this.listener,!1)}),u.on("xhr-cb-time",function(t,e,n){this.cbTime+=t,e?this.onloadCalled=!0:this.called+=1,this.called!==this.totalCbs||!this.onloadCalled&&"function"==typeof n.onload||this.end(n)}),u.on("xhr-load-added",function(t,e){var n=""+p(t)+!!e;this.xhrGuids&&!this.xhrGuids[n]&&(this.xhrGuids[n]=!0,this.totalCbs+=1)}),u.on("xhr-load-removed",function(t,e){var n=""+p(t)+!!e;this.xhrGuids&&this.xhrGuids[n]&&(delete this.xhrGuids[n],this.totalCbs-=1)}),u.on("addEventListener-end",function(t,e){e instanceof m&&"load"===t[0]&&u.emit("xhr-load-added",[t[1],t[2]],e)}),u.on("removeEventListener-end",function(t,e){e instanceof m&&"load"===t[0]&&u.emit("xhr-load-removed",[t[1],t[2]],e)}),u.on("fn-start",function(t,e,n){e instanceof m&&("onload"===n&&(this.onload=!0),("load"===(t[0]&&t[0].type)||this.onload)&&(this.xhrCbStart=(new Date).getTime()))}),u.on("fn-end",function(t,e){this.xhrCbStart&&u.emit("xhr-cb-time",[(new Date).getTime()-this.xhrCbStart,this.onload,e],e)})}},{}],11:[function(t,e,n){e.exports=function(t){var e=document.createElement("a"),n=window.location,r={};e.href=t,r.port=e.port;var o=e.href.split("://");!r.port&&o[1]&&(r.port=o[1].split("/")[0].split("@").pop().split(":")[1]),r.port&&"0"!==r.port||(r.port="https"===o[0]?"443":"80"),r.hostname=e.hostname||n.hostname,r.pathname=e.pathname,r.protocol=o[0],"/"!==r.pathname.charAt(0)&&(r.pathname="/"+r.pathname);var i=!e.protocol||":"===e.protocol||e.protocol===n.protocol,a=e.hostname===document.domain&&e.port===n.port;return r.sameOrigin=i&&(!e.hostname||a),r}},{}],12:[function(t,e,n){function r(t,e){return function(){o(t,[(new Date).getTime()].concat(a(arguments)),null,e)}}var o=t("handle"),i=t(14),a=t(15);"undefined"==typeof window.newrelic&&(newrelic=NREUM);var s=["setPageViewName","setCustomAttribute","finished","addToTrace","inlineHit"],c=["addPageAction"],f="api-";i(s,function(t,e){newrelic[e]=r(f+e,"api")}),i(c,function(t,e){newrelic[e]=r(f+e)}),e.exports=newrelic,newrelic.noticeError=function(t){"string"==typeof t&&(t=new Error(t)),o("err",[t,(new Date).getTime()])}},{}],13:[function(t,e,n){var r=0,o=navigator.userAgent.match(/Firefox[\/\s](\d+\.\d+)/);o&&(r=+o[1]),e.exports=r},{}],14:[function(t,e,n){function r(t,e){var n=[],r="",i=0;for(r in t)o.call(t,r)&&(n[i]=e(r,t[r]),i+=1);return n}var o=Object.prototype.hasOwnProperty;e.exports=r},{}],15:[function(t,e,n){function r(t,e,n){e||(e=0),"undefined"==typeof n&&(n=t?t.length:0);for(var r=-1,o=n-e||0,i=Array(0>o?0:o);++r<o;)i[r]=t[e+r];return i}e.exports=r},{}],16:[function(t,e,n){function r(t){return!(t&&"function"==typeof t&&t.apply&&!t[a])}var o=t("ee"),i=t(15),a="nr@original",s=Object.prototype.hasOwnProperty,c=!1;e.exports=function(t){function e(t,e,n,o){function nrWrapper(){var r,a,s,c;try{a=this,r=i(arguments),s="function"==typeof n?n(r,a):n||{}}catch(u){d([u,"",[r,a,o],s])}f(e+"start",[r,a,o],s);try{return c=t.apply(a,r)}catch(l){throw f(e+"err",[r,a,l],s),l}finally{f(e+"end",[r,a,c],s)}}return r(t)?t:(e||(e=""),nrWrapper[a]=t,u(t,nrWrapper),nrWrapper)}function n(t,n,o,i){o||(o="");var a,s,c,f="-"===o.charAt(0);for(c=0;c<n.length;c++)s=n[c],a=t[s],r(a)||(t[s]=e(a,f?s+o:o,i,s))}function f(e,n,r){if(!c){c=!0;try{t.emit(e,n,r)}catch(o){d([o,e,n,r])}c=!1}}function u(t,e){if(Object.defineProperty&&Object.keys)try{var n=Object.keys(t);return n.forEach(function(n){Object.defineProperty(e,n,{get:function(){return t[n]},set:function(e){return t[n]=e,e}})}),e}catch(r){d([r])}for(var o in t)s.call(t,o)&&(e[o]=t[o]);return e}function d(e){try{t.emit("internal-error",e)}catch(n){}}return t||(t=o),e.inPlace=n,e.flag=a,e}},{}],ee:[function(t,e,n){function r(){}function o(t){function e(t){return t&&t instanceof r?t:t?s(t,a,i):i()}function n(n,r,o){t&&t(n,r,o);for(var i=e(o),a=l(n),s=a.length,c=0;s>c;c++)a[c].apply(i,r);var u=f[v[n]];return u&&u.push([w,n,r,i]),i}function d(t,e){m[t]=l(t).concat(e)}function l(t){return m[t]||[]}function p(t){return u[t]=u[t]||o(n)}function h(t,e){c(t,function(t,n){e=e||"feature",v[n]=e,e in f||(f[e]=[])})}var m={},v={},w={on:d,emit:n,get:p,listeners:l,context:e,buffer:h};return w}function i(){return new r}var a="nr@context",s=t("gos"),c=t(14),f={},u={},d=e.exports=o();d.backlog=f},{}],gos:[function(t,e,n){function r(t,e,n){if(o.call(t,e))return t[e];var r=n();if(Object.defineProperty&&Object.keys)try{return Object.defineProperty(t,e,{value:r,writable:!0,enumerable:!1}),r}catch(i){}return t[e]=r,r}var o=Object.prototype.hasOwnProperty;e.exports=r},{}],handle:[function(t,e,n){function r(t,e,n,r){o.buffer([t],r),o.emit(t,e,n)}var o=t("ee").get("handle");e.exports=r,r.ee=o},{}],id:[function(t,e,n){function r(t){var e=typeof t;return!t||"object"!==e&&"function"!==e?-1:t===window?0:a(t,i,function(){return o++})}var o=1,i="nr@id",a=t("gos");e.exports=r},{}],loader:[function(t,e,n){function r(){if(!m++){var t=h.info=NREUM.info,e=u.getElementsByTagName("script")[0];if(t&&t.licenseKey&&t.applicationID&&e){c(l,function(e,n){t[e]||(t[e]=n)});var n="https"===d.split(":")[0]||t.sslForHttp;h.proto=n?"https://":"http://",s("mark",["onload",a()],null,"api");var r=u.createElement("script");r.src=h.proto+t.agent,e.parentNode.insertBefore(r,e)}}}function o(){"complete"===u.readyState&&i()}function i(){s("mark",["domContent",a()],null,"api")}function a(){return(new Date).getTime()}var s=t("handle"),c=t(14),f=window,u=f.document;NREUM.o={ST:setTimeout,CT:clearTimeout,XHR:f.XMLHttpRequest,REQ:f.Request,EV:f.Event,PR:f.Promise,MO:f.MutationObserver},t(12);var d=""+location,l={beacon:"bam.nr-data.net",errorBeacon:"bam.nr-data.net",agent:"js-agent.newrelic.com/nr-943.min.js"},p=window.XMLHttpRequest&&XMLHttpRequest.prototype&&XMLHttpRequest.prototype.addEventListener&&!/CriOS/.test(navigator.userAgent),h=e.exports={offset:a(),origin:d,features:{},xhrWrappable:p};u.addEventListener?(u.addEventListener("DOMContentLoaded",i,!1),f.addEventListener("load",r,!1)):(u.attachEvent("onreadystatechange",o),f.attachEvent("onload",r)),s("mark",["firstbyte",a()],null,"api");var m=0},{}]},{},["loader",2,10,4,3]);</script><script type="text/javascript">window.NREUM||(NREUM={});NREUM.info={"beacon":"bam.nr-data.net","queueTime":0,"licenseKey":"750e9545e9","agent":"","transactionName":"blABZhZZVkdUBhdbXVcaJUcKW0xdWgtMU1xOUAEcElFdQ0ZLEEdAT1AabRdNVVlUFxoIQUxHFVcdZ0tBWAgCQEs=","applicationID":"4303722","errorBeacon":"bam.nr-data.net","applicationTime":319}</script>
        <meta name="msapplication-config" content="none"/>
        <meta name="keywords" content="questionnaire, questionnaires, questionaire, questionaires, free online survey, free online surveys" />
        <meta name="description" content="Create and publish online surveys in minutes, and view results graphically and in real time. SurveyMonkey provides free online questionnaire and survey software." />
        <meta name="author" content="SurveyMonkey">
        
        

        

        <!--[if lt IE 9]>
            <script src="https://secure.surveymonkey.com/smassets/anweb/smlib.ui-html5-bundle-min.a7370863.js" 
    ></script>
        <![endif]-->

        
            <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/smlib.ui-global-bundle-min.0aca324d.css" 
     />
        

        
<!--[if lte IE 9]>
<link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates-base_nonresponsive-bundle-min.5f068e35.css" 
     />
<![endif]-->
<!--[if (gt IE 9)|(!IE)]><!-->

<link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates-base_nonresponsive-bundle-min.5f068e35.css" 
     />

<!--<![endif]-->

        

        
            
                <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc-top_bar-bundle-min.e24b7bd5.css"/>
            
                <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc-survey_summary-bundle-min.2fea2090.css"/>
            
        

        
    <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/smlib.ui-global-pro-bundle-min.58ab10f2.css" 
     />
    <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/anweb-survey-summary-bundle-min.0f953009.css" 
     />
    <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/anweb-upgrades-bundle-min.aae7f287.css" 
     />
    <link type="text/css" rel="stylesheet" href="https://secure.surveymonkey.com/smassets/anweb/anweb-upgrade-slide-dialog-bundle-min.7d0bb631.css" 
     />



        <link rel="shortcut icon" href="/favicon1.ico" />
        <link rel="image_src" href="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/sm_logo_fb.png" />
        <!-- image icon if website is saved to iOS home screen -->
        <link rel="apple-touch-icon" href="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/sm_logo_fb.png">
    </head>

    <!--[if lt IE 7 ]>
    <body class="translate  ie6">
    <![endif]-->
    <!--[if IE 7 ]>
    <body class="translate  ie7">
    <![endif]-->
    <!--[if IE 8 ]>
    <body class="translate  ie8">
    <![endif]-->
    <!--[if IE 9 ]>
    <body class="translate  ie9">
    <![endif]-->
    <!--[if (gt IE 9)|(!IE)]><!-->
    <body class="translate  modern-browser not-mobile-ready">
    <!--<![endif]-->
        
        
        
            
        

        <div class="content-wrapper">

            
                

<div class="base-header auth-header" id="hd">
  
  <div class="inner-header clearfix">
    <div class="inner-header-top clearfix">
      <ol class="user-area">
        
          
            <li class="yel"><a href="/pricing/?ut_source=header_upgrade&ut_source2=wide_menu" data-sl-variant="upgrade-now-insights">Upgrade</a></li>
          
          <li class="has-submenu" id="dd-my-account">
            <ul>
              <li class="first-item">
                <a href="#" id="userAcctTab_MainMenu2" class="hd notranslate">
                  surveyfsa@gmail.com
                  <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" align="top" />
                </a>
              </li>
              
              <li><a href="/user/account/">My Account</a></li>
              <li><a href="/addressbook/">Contacts</a></li>
              <li><a class="help" href="http://help.surveymonkey.com/?l=en_US&amp;uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" target="_blank">Help Center</a></li>
              <li class="last"><a href="/user/sign-out/">Sign Out</a></li>
            </ul>
            <a href="#" id="userAcctTab_MainMenu" class="hd notranslate">
              surveyfsa@gmail.com
              <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" align="top" />
            </a>
          </li>
        
      </ol>
      <a class="responsive-logo" href="/">
    <span class="logo">SurveyMonkey&reg;</span>

    <div class="hamburger-menu">
        <span class="hamburger-line top-line close-hidden"></span>
        <span class="hamburger-line middle-line close-up"></span>
        <span class="hamburger-line middle-line close-down"></span>
        <span class="hamburger-line bottom-line close-hidden"></span>
    </div>

    

    <span class="smf-icon small-mobile-logo">÷</span>

    <object data="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/logo/surveymonkey_logo_dark.svg" type="image/svg+xml" alt="SurveyMonkey Logo">
        <!--[if lte IE 8]>
            <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/logo/surveymonkey_logo_dark_low.png" alt="SurveyMonkey Logo">
        <![endif]-->
        <!--[if !IE]> -->
            <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/logo/surveymonkey_logo_dark_low.png" alt="SurveyMonkey Logo"/>
        <!-- <![endif]-->
    </object>
</a>
    </div>
    
      <ol class="nav clearfix">
        <li>
          <a href="/home/?ut_source=header" class="first-item ">My Surveys</a>
        </li>
        
        
        <li class="has-submenu" id="dd-online-surveys">
          <div class="hd-bg">
            <a href="#" id="surveysTab_MainMenu" class="hd ">
              Examples
              <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" />
            </a>
          </div>
          <ul class="nav-submenu">
            <li><a href="/mp/survey-templates/?ut_source=header">Survey Templates</a></li>
            <li><a href="/mp/survey-guidelines/?ut_source=header">Survey Tips</a></li>
            <li><a href="/mp/survey-types/?ut_source=header">Survey Types</a></li>
            <li><a href="/mp/academic-surveys/?ut_source=header">Academic Research</a></li>
            <li><a href="/mp/customer-satisfaction-surveys/?ut_source=header">Customer Satisfaction</a></li>
            <li><a href="/mp/education-surveys/?ut_source=header">Education</a></li>
            <li><a href="/mp/employee-surveys/?ut_source=header">Employee</a></li>
            <li><a href="/mp/healthcare-surveys/?ut_source=header">Healthcare</a></li>
            <li><a href="/mp/market-research-surveys/?ut_source=header">Market Research</a></li>
            <li><a href="/mp/non-profit-surveys/?ut_source=header">Non Profit</a></li>
            <li><a href="/mp/event-planning-surveys/?ut_source=header">Events</a></li>
            <li class="min-width"><img class="img" width="200" height="2" src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" /></li>
          </ul>
        </li>
        <li class="has-submenu" id="dd-use-cases">
          <div class="hd-bg">
            <a href="#" id="resourceTab_MainMenu" class="hd ">
              Survey Services
              <img src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" />
            </a>
          </div>
          <ul class="nav-submenu">
            <li class="SL_hide"><a href="/mp/audience/?ut_source=sma&ut_source2=web_header">Buy Survey Responses</a></li>
            
            
            <li><a href="/mp/enterprise/?ut_source=ent&ut_source2=web_header">Buy a Multi-User Account</a></li>
            <li class="SL_hide"><a href="/mp/benchmarks/?ut_source=bmk&ut_source2=web_header">Get Benchmarks</a></li>
            <li class="SL_swap" id="topnav-iphoneapp"><a href="/mp/iphone-survey-app/?ut_source=header">Mobile App</a></li>
            <li class="SL_hide"><a href="/integrations/?ut_source=header">Integrations</a></li>
            <li class="SL_hide"><a href="https://contribute.surveymonkey.com/?ut_source=header" target="_blank">Take Surveys</a></li>
            <li class="SL_hide"><a href="/mp/wufoo-online-forms/?ut_source=header">Wufoo Online Forms</a></li>
            
            <li class="SL_hide"><a href="/business/intelligence/?utm_source=product&utm_medium=nav&utm_content=launch_promo&utm_campaign=smi">Mobile Intelligence</a></li>
            
            <li class="min-width"><img class="img" width="200" height="2" src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates/4.1.2/assets/t.gif" /></li>
          </ul>
        </li>
        <li>
          <a href="/pricing/upgrade/quickview?ut_source=header_loggedIn" >Plans & Pricing</a>
        </li>
      </ol>
      
        <a href="/create/?ut_source=create_survey&ut_source2=header" class="create-survey btn green SL_split">+ Create Survey</a>
        <a href="/create/?ut_source=create_survey&ut_source2=headerfab" class="create-survey fab SL_split" title="Create Survey">+</a>
      
    
  </div>
</div>
            

            
                
<div id="ucs-reinstate-success-notification" class="notification" test-id="global_autorenew_off_slim">
<div class="sm-notification-icon smf-icon">2</div>
<div class="sm-notification-message">
<h3>Your changes have been saved</h3>
</div>
</div>
<div id="ucs-reinstate-error-notification" class="notification error">
<div class="sm-notification-icon smf-icon">!</div>
<div class="sm-notification-message">
<h3>Oops, something went wrong</h3>
</div>
</div>
<section id="ucs-autorenew" data-notifications-js="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc-notifications-bundle-min.ef0682e4.js" data-notification-css="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc-notifications-bundle-min.eb059e23.css" class="ucs-module ucs-module-topbar-slim hot">
<span class="headline">Before you forget!</span> Keep access to your survey data and paid features. 
        <a href="#" id="ucs-reinstate-autorenew">Enable Auto-renew</a>
</section>

            

            
    <div class="survey-header-container">
        <div class="survey-header-inner-container clearfix">
        	
                
    
    
    
    <div class="survey-header clearfix">
        
        <div class="survey-header-title-container notranslate">
            <h2 class="survey-header-title">Parent Survey</h2>
        </div>
        <ul class="survey-header-tabs clearfix">
            <li class=" sm-corner-t">
                <a href="/analyze/VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" data-location="analyze">
                    Analyze Results
                </a>
            </li>
            <li class=" sm-corner-t">
                <a href="/collect/list?sm=VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" data-location="collect">
                    Collect Responses
                </a>
            </li>
            <li class=" sm-corner-t">
                <a href="/create/?sm=VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" data-location="create">
                    Design Survey
                </a>
            </li>
            
                <li class=" selected  sm-corner-t">
                    <a href="/summary/VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" data-location="summary">Summary</a>
                </li>
            
        </ul>
    </div>

        	
        </div>
    </div>


            <div class="bd logged-in-bd">
                <div class="container clearfix">
                    
    <div class="survey-summary-layout clearfix" survey-summary-layout></div>
    
    <a id="feedbackTab" class="pop sidetab" title="Tell us what you think!" sm-tooltip-side="left" href="https://www.surveymonkey.com/r/9GXBVRF?c=VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" target="_blank">
      Feedback
    </a>

    <div id="javascript-templates" style="display: none">
        <script type="text/html" id="status-notification-template">
    <div class="sm-notification <%classes%>">
        <div class="sm-notification-icon smf-icon"><%icon%></div>
        <div class="sm-notification-message">
            <h3 class="sm-notification-message-title"><%&title%></h3>
            <%#message%>
                <p class="sm-notification-message-content"><%&message%></p>
            <%/message%>
            <%#content%>
                <div class="sm-notification-message-custom-content"><%&content%></div>
            <%/content%>
        </div>
        <a href="#" notification-close-btn class="main-close-btn smf-icon">D</a>
    </div>
</script>

<script type="text/html" id="notifications-container-template">
    <div class="sm-notification-container"></div>
</script>

<script type="text/html" id="notification-wrapper-template">
    <div class="sm-notification-wrapper"></div>
</script>

<script type="text/html" id="notification-template">
    <div class="sm-notification"></div>
</script>
        <script type="text/html" id="dialog-title-bar-template">
    <div class="dialog-title-bar">
        <h5><%title%></h5>
    </div>
</script>
<script type="text/html" id="dialog-close-btn-template">
    <a class="dialog-close-btn cbmain smf-icon" href="#">D</a>
</script>
<script type="text/html" id="dialog-overlay-template">
    <div class="dialog-overlay<%#isModal%> dialog-overlay-modal<%/isModal%>"></div>
</script>
<script type="text/html" id="dialog-container-template">
    <div class="dialog-container"></div>
</script>
        <script type="text/html" id="upgrade-slide-dialog-template">
  <div class="dialog dialog-a upgradeModal">
    <%#hasMany%>
	    <a href="#" prev-btn class="prev">Previous<span class="upgrade-nav-arrow">Æ</span></a>
	    <a href="#" next-btn class="next">Next<span class="upgrade-nav-arrow">ÿ</span></a>
	<%/hasMany%>
    <section>
    </section>
    <div class="dialog-btn-bar clearfix">
	    <%#hasMany%>
			<nav>
			    <%#slides%>
			        <a slide-index="<%index%>" href="#">
			            <%position%>
			        </a>
			    <%/slides%>
			</nav>
		<%/hasMany%>
		<a upgrade-btn class="btn yellow btn-txt-primary upgrade-button" href="#">
			Upgrade
		</a>
    </div>
  </div>
</script>
        <script type="text/html" id="action-menu-template">
    <ul class="option-menu action-menu">
        <%#actions%>
            <li>
                <a href="#" class='option <%#isDisabled%>disabled<%/isDisabled%>' data-action="<%action%>"><%text%></a>
            </li>
        <%/actions%>
    </ul>
</script>
        
        
        
	    <script id="upgradeProTemplates" type="text/html">
		<div class="clearfix upgradeProTemplates" upgrade-url="/pricing/?ut_source=wall_surveytemplates&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Pro templates.</h2>
   			<h3>Ask like an expert.</h3>
   			<p>Ask questions like an expert with our <b>certified templates</b> from our team of methodologists.</p>
   			<p>Availible with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeMaxQuestions" type="text/html">
		<div class="clearfix upgradeMaxQuestions" upgrade-url="/pricing/?ut_source=wall_maxquestions&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Unlimited questions.</h2>
   			<h3>Don&#39;t be left wondering.</h3>
   			<p>Break through the 10 question limit of our BASIC plan and <b>add unlimited questions</b> to your survey.</p>
   			<p>Availible with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeLogo" type="text/html">
		<div class="clearfix upgradeLogo" upgrade-url="/pricing/?ut_source=wall_logo&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Add a logo.</h2>
   			<h3>Show off your brand.</h3>
   			<p><b>Add your logo</b> to your survey and provide your respondents with brand continuity.</p>
   			<p>Available with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradePageLogic" type="text/html">
		<div class="clearfix upgradePageLogic" upgrade-url="/pricing/?ut_source=wall_pageskiplogic&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Page Skip logic.</h2>
   			<h3>Redirect unconditionally</h3>
   			<p><b>Redirect respondents</b> to another page of your survey.</p>
   			<p>Available with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeQuestionLogic" type="text/html">
		<div class="clearfix upgradeQuestionLogic" upgrade-url="/pricing/?ut_source=wall_questionskiplogic&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Skip logic.</h2>
   			<h3>If this, then that.</h3>
   			<p><b>Redirect respondents</b> to another page of your survey based on their answer.</p>
   			<p>Available with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradePageRandom" type="text/html">
		<div class="clearfix upgradePageRandom" upgrade-url="/pricing/?ut_source=wall_page_randomization&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Page Randomization.</h2>
   			<h3>Shuffle your survey pages.</h3>
   			<p><b>Randomize, flip or rotate</b> the pages of your survey to minimize order bias.</p>
   			<p>Available with <strong>GOLD</strong> or <strong>PLATINUM</strong> plans.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeQuestionRandom" type="text/html">
		<div class="clearfix upgradeQuestionRandom" upgrade-url="/pricing/?ut_source=wall_question_randomization&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Question Randomization</h2>
   			<h3>Shuffle your questions.</h3>
   			<p><b>Randomize, or flip</b> the questions on a survey page to minimize selection bias.</p>
   			<p>Available with <strong>GOLD</strong> or <strong>PLATINUM</strong> plans.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeQuotas" type="text/html">
		<div class="clearfix upgradeQuotas" upgrade-url="/pricing/?ut_source=wall_quotas&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Quotas</h2>
   			<h3>Screen out your respondents.</h3>
   			<p><b>Set quota limits</b> on how many responses you receive for specific questions in your survey.</p>
   			<p>Available with any <strong>GOLD</strong> or <strong>PLATINUM</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeCustomVariables" type="text/html">
		<div class="clearfix upgradeCustomVariables" upgrade-url="/pricing/?ut_source=wall_custom_variables&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Custom Variables</h2>
   			<h3>Personalize your surveys.</h3>
   			<p>Setup custom variables to <b>pass pre-collected data</b> about your respondents into your survey.</p>
   			<p>Available with a <strong>PLATINUM</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeThemes" type="text/html">
		<div class="clearfix upgradeThemes" upgrade-url="/pricing/?ut_source=wall_themes&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Custom Themes.</h2>
   			<h3>Unleash your inner designer.</h3>
   			<p><b>Customize your surveys colors &amp; fonts</b> for a more distinctive look and branded feel.</p>
   			<p>Available with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradePrint" type="text/html">
		<div class="clearfix upgradePrint" upgrade-url="/pricing/?ut_source=wall_print&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Printable surveys.</h2>
   			<h3>Sometimes paper is better.</h3>
   			<p><b>Create a printable version</b> of your survey in PDF format.</p>
   			<p>Available with any <strong>PRO</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeFooter" type="text/html">
		<div class="clearfix upgradeFooter" upgrade-url="/pricing/?ut_source=wall_footer&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Hide our standard footer.</h2>
   			<h3>We&#39;ll be your silent partner.</h3>
   			<p><b>Hide our standard "Powered by SurveyMonkey" footer</b> on your survey.</p>
   			<p>Available with any <strong>GOLD</strong> or <strong>PLATINUM</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradePiping" type="text/html">
		<div class="clearfix upgradePiping" upgrade-url="/pricing/?ut_source=wall_piping&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Question piping.</h2>
   			<h3>Create personalized surveys.</h3>
   			<p>Piping is a feature used to <b>customize questions with your respondent's previous answers</b> using our survey templating tags.</p>
   			<p>Available with any <strong>GOLD</strong> or <strong>PLATINUM</strong> plan.</p>
         </div>
		</div>
	</script>
	
	    <script id="upgradeRandomAssignment" type="text/html">
		<div class="clearfix upgradeRandomAssignment" upgrade-url="/pricing/?ut_source=wall_random_assignment&amp;ut_source2=ssum">
			<span class="thumbnail"></span>
         <div class="upgradeInfo">
   			<h2>Random Assignment.</h2>
   			<h3>Run an A/B test in your survey and measure the effect of varying your text or images.</h3>
   			<p></p>
   			<p>Available with any <strong>GOLD</strong> or <strong>PLATINUM</strong> plan.</p>
         </div>
		</div>
	</script>
	

        <script type="text/html" id="upgrade-browser-warning-dialog-template">
    <div class="dialog upgrade-browser-warning-dialog">
        <div class="clearfix">
            <div class="content sm-float-l">
                <div class="clearfix">
                    <div class="warning-icon sm-float-l">
                        <span class="smf-icon">!</span>
                    </div>
                    <div class="headings sm-float-l">
                        <h2>Update Your Browser</h2>

                        <h3>Make sure all of our features work.</h3>
                    </div>
                </div>
                <div class="main-content">
                    <p>We stay up-to-date to get you the best results, but your web browser is behind the times. Be
                        warned: some of our features won&#39;t work for you! Choose a browser below to get up to
                        speed.</p>

                    <ul class="browser-icons">
                        <li data-browser="chrome">
                            <a href="http://www.google.com/chrome" target="_blank">
                                <span>Chrome</span>
                            </a>
                        </li>
                        <li data-browser="firefox">
                            <a href="http://www.mozilla.org/firefox/fx/#desktop" target="_blank">
                                <span>Firefox</span>
                            </a>
                        </li>
                        <li data-browser="safari">
                            <a href="http://www.apple.com/safari/download/" target="_blank">
                                <span>Safari</span>
                            </a>
                        </li>
                        <li data-browser="opera">
                            <a href="http://www.opera.com/download/" target="_blank">
                                <span>Opera</span>
                            </a>
                        </li>
                        <li data-browser="ie">
                            <a href="http://www.microsoft.com/windows/Internet-explorer/default.aspx" target="_blank">
                                <span>Internet Explorer</span>
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</script>
        <script type="text/html" id="img">
    <img class="<% classes %>" src="<% src %>" alt="<% alt %>" title="<% title %>"/>
</script>
        <script type="text/html" id="no-questions-template">
    <div class="sm-corner-a no-content analyze-null-state txt-shadow-lt no-survey-questions-message <%classes%>">
        <h3 class="no-content-title txt-shadow-lt">
            <span class="header-icon pictos">!</span> Add questions to your survey
        </h3>

        <div class="button-bar spacer-mtl">
            <a href="/create/?sm=<%&surveyIDEncryption%>" class="btn large teal">+ Add Questions</a>
        </div>
    </div>
</script>

<script type="text/html" id="no-responses-template">
    <div class="sm-corner-a no-content analyze-null-state txt-shadow-lt <%classes%>">

        <h3 class="no-content-title txt-shadow-lt">
            <span class="header-icon pictos">!</span>
            <%# onSharedPage %>This survey has no responses<%/ onSharedPage %>
            <%^ onSharedPage %>Your survey has no responses<%/ onSharedPage %>
        </h3>

        <%^ onSharedPage %>
        <div class="button-bar spacer-mtl">
            <a href="/collect/list?sm=<%&surveyIDEncryption%>" class="btn large teal">Collect
                responses</a>
            <%# shouldShowBuyResponsesButton %>
            <span class="or">OR</span>
            <a href="/collect/audience/getstarted/?ut_source=sma&ut_source2=li_analyze&survey_id=<%surveyID%>"
               class="btn large yellow">Buy responses</a>
            <%/ shouldShowBuyResponsesButton %>
        </div>
        <%/ onSharedPage %>
    </div>
</script>

<script type="text/html" id="content-load-error-template">
    <div class="sm-corner-a no-content analyze-null-state txt-shadow-lt <%classes%>">
        <h3 class="no-content-title txt-shadow-lt">
            <span class="header-icon pictos">!</span> Rotten Bananas!
        </h3>

        <div class="no-content-content">
            <p>
                There was an issue getting your responses. In the meantime, please visit our <a href="/help/">Help
                Desk</a>
                for more information on analyzing results.
            </p>

            <div class="sm-float-r">
                <%#errorCode%>Error Code: <%errorCode%><%/errorCode%>
                <%#requestID%>Request ID: <%requestID%><%/requestID%>
            </div>
        </div>
    </div>
</script>

<script type="text/html" id="view-switch-failed">
    <div class="sm-corner-a no-content analyze-null-state txt-shadow-lt <%classes%>">
        <h3 class="no-content-title txt-shadow-lt">
            <span class="header-icon pictos">!</span> Rotten Bananas!
        </h3>

        <div class="no-content-content">
            <p>
                We had a problem loading your view.
            </p>

            <p>
                We appreciate your patience.
            </p>
            <%#requestID%>
            <div class="sm-float-r">Error ID: <%requestID%></div>
            <%/requestID%>
        </div>
    </div>
</script>

<script type="text/html" id="filtered-no-responses-template">
    <div class="sm-corner-a no-content analyze-null-state txt-shadow-lt <%classes%>">
        <h3 class="no-content-title txt-shadow-lt">
            <span class="header-icon pictos">!</span> No Matching Responses
        </h3>

        <div class="no-content-content">
            <p>
                None of your responses meet the criteria of your filter rules. To view your responses edit or deselect your filter rules.
            </p>
        </div>
    </div>
</script>

<script type="text/html" id="no-page-questions">
    <div class="no-questions-page sm-corner-a">
        There are no questions on this page.
    </div>
</script>

<script type="text/html" id="no-shown-page-questions">
    <div class="no-questions-page sm-corner-a">
        There are no shown questions. Edit your show rule to view your responses.
    </div>
</script>
        <script type="text/html" id="analyze-content-loader-template">
    <div analyze-content-loader class="analyze-content-loader spacer-pal hide">
        <img alt="Loading" src="https://secure.surveymonkey.com/smassets/anweb/smlib.ui/2.1.0/assets/spiffygif_66x66.gif"/>
        <div class="loading-text">Loading ...</div>
    </div>
</script>
        <script type="text/html" id="analyze-quotas-header-template">
    <div class="quotas-container">
        <div class="accordion">
            <div class="quotas-header-container key">
                <header>
                    <h3>
                        <div class="quotas-header clearfix sm-float-t txt-shadow-dark">
                            <a class="keyOpener" href="#" target="#QuotasViewContainer">
                                <div class="quota-description">
                                    QUOTA STATUS <span class="num-quotas subtitle">(<%numQuotas%>)</span>
                                </div>
                                <div class="progress-bar-section">
                                    <div id="progress-bar-main">
                                        <div class="progress-bar-container-header">
                                            <div class="progress-bar"></div>
                                        </div>
                                        <div class="progress-bar-percent"> <%totalPercent%> </div>
                                    </div>
                                </div>
                            </a>
                        </div>
                    </h3>
                    <div class="q q-on-dark">
                        <span>?</span>
                        <div class="popout">
                            <h5>QUOTA PROGRESS</h5>
                            <p>You have set up one or more quotas for your survey. You can see the progress of your quota responses here. To edit your quotas, go back to &ldquo;Design&rdquo;.</p>
                            <a class="learn-more-link" target="_blank" href="http://help.surveymonkey.com/articles/en_US/kb/What-are-Quotas?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D#quotas">Learn more &raquo;</a>
                        </div>
                    </div>
                </header>
                <section id="QuotasViewContainer">
                </section>
            </div>
        </div>
    </div>
</script>
        <script type="text/html" id="analyze-quotas-template">
        <div class="quota-section">
            <div class="quota-description">
                Quota <%quota_name%>: <%totalContext%> of <%total%>
            </div>
            <div class="progress-bar-section">
                <div class="progress-bar-container">
                    <div class="progress-bar"></div>
                </div>
                <div class="progress-bar-percent"> <%percent%> </div>
                <div class="section-holder"></div>
            </div>
        </div>
</script>

<script type="text/html" id="analyze-quotas-list-template">
    <div id="QuotasListView">
    </div>
</script>
        <script id="survey-summary-container-template" type="text/html">
    <div class="survey-summary-container"></div>
</script>
<script id="survey-notification-acknowledge-template" type="text/html">
    <div class="acknowledge">
        <div class="ack-checked-icon smf-icon">2</div>
        <div><span class="ack-message-title">Success!</span>&nbsp;<span class="ack-message-content">Survey Alerts for this survey is now off.</span></div>
        <a href="#" acknowledge-close-btn class="ack-close-btn smf-icon">D</a>
    </div>
</script>
        
<script id="survey-details-template" type="text/html">
	<div class="secondary">
		<div class="mod survey-details-container">
		    <header class="mod-header clearfix">
		        <h3 class="sm-float-l txt-shadow-dark"><span class="all-caps">Design Summary</span></h3>
		    </header>
		    <div class="mod-body">
			    <div class="sm-grid survey-details-title-container">
			        <div class="sm-grid-block sm-grid-block-row-start sm-grid-block-20">
			            <a href="/create/?sm=<%encryptedID%>">
			            	<img alt="Survey Icon" class="survey-details-icon" src="https://secure.surveymonkey.com/smassets/anweb/anweb/88.5.247/assets/survey-icon.png"/>
                        </a>
			        </div>
			        <div class="sm-grid-block sm-grid-block-80">
			            <a href="/create/?sm=<%encryptedID%>">
			                <h4 class="spacer-mbs survey-details-survey-title">
			                    <% title %>
			                </h4>
		                </a>
		                <div class="negative">
                            Created on <%dateCreated%>
		                </div>
			        </div>
			    </div>
				<div class="survey-feature-checklist">
				    <div class="survey-feature-row">
				        <%#hasQuestions%>
						    <span class="smf-icon">3</span> Questions: <span class="detail-count"><% fullQuestionCount %></span>, Pages: <span class="detail-count"><% pageCount %></span>
				        <%/hasQuestions%>
				        <%^hasQuestions%>
				            <span class="negative">
				                No questions added
				            </span>
				        <%/hasQuestions%>
				    </div>
				    <div class="survey-feature-row">
				        <span class="smf-icon">3</span> Survey language: <%language%>
				    </div>
				    <div class="survey-feature-row">
				        <%#theme%>
				            <span class="smf-icon">3</span> Theme: <%theme%>
				        <%/theme%>
				        <%^theme%>
				            <span class="negative">
				                No theme added
				            </span>
				        <%/theme%>
				    </div>
				    <div class="survey-feature-row <%^logoEnabled%> survey-feature-upgrade <%/logoEnabled%>" <%^logoEnabled%>upgrade-id="upgradeLogo"<%/logoEnabled%>>
				        <%#logoEnabled%>
					        <%#logoAdded%>
					            <span class="smf-icon">3</span> Logo added
					        <%/logoAdded%>
					        <%^logoAdded%>
					            <span class="negative">
					                No logo added
					            </span>
					            <div class="q sm-float-r" data-help="no-logo-popout-template">
				        		    <span>?</span>
				                </div>
					        <%/logoAdded%>
				        <%/logoEnabled%>
				        <%^logoEnabled%>
                            Upgrade to add your logo
                            <div class="q sm-float-r" data-help="upgrade-logo-popout-template">
			        		    <span>?</span>
			                </div>
				        <%/logoEnabled%>
				    </div>
				    <div class="survey-feature-row <%^logicEnabled%> survey-feature-upgrade <%/logicEnabled%> <%^hasQuestions%> sm-corner-b <%/hasQuestions%>" <%^logicEnabled%>upgrade-id="upgradePageLogic"<%/logicEnabled%>>
					    <%#logicEnabled%>
					        <%#logicAdded%>
					            <span class="smf-icon">3</span> Logic added
					        <%/logicAdded%>
					        <%^logicAdded%>
					            <span class="negative">
					                No logic added
					            </span>
					            <div class="q sm-float-r" data-help="no-logic-popout-template">
				        		    <span>?</span>
				                </div>
					        <%/logicAdded%>
					    <%/logicEnabled%>
					    <%^logicEnabled%>
                            Upgrade to add logic
                            <div class="q sm-float-r" data-help="upgrade-logic-popout-template">
			        		    <span>?</span>
			                </div>
				        <%/logicEnabled%>
				    </div>
				</div>
				<%#hasQuestions%>
				    <div class="survey-design-actions">
				        <a href="/create/?sm=<%encryptedID%>" class="btn btn-small">
				            Edit Design
				        </a>
				        <a href="<%previewLink%>" class="btn btn-small" target="_blank">
				            Preview Survey
				        </a>
				    </div>
		        <%/hasQuestions%>
		    </div>
		</div>
	</div>
</script>





<script id="no-logo-popout-template" type="text/html">
  

  <h5>ADD A LOGO</h5>
  <p>You can add your logo to a survey. Your logo will appear at the top of your survey. You can choose to align it left or center.</p>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/How-do-I-add-or-edit-a-logo?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">
  
    Learn more »
  
  </a>

  

  

  

  

</script>

<script id="no-logic-popout-template" type="text/html">
  

  <h5>ADD LOGIC</h5>
  <p>You can create powerful surveys by adding logic including Question Skip Logic, Page Randomization, Question Randomization,	and more.</p>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/How-do-I-create-conditional-skip-logic?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">
  
    Learn more »
  
  </a>

  

  

  

  

</script>

<script id="upgrade-logo-popout-template" type="text/html">
  

  <h5>ADD A LOGO</h5>
  <p>You can add your logo to a survey. Your logo will appear at the top of your survey. You can choose to align it left or center.</p>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/How-do-I-add-or-edit-a-logo?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">
  
    Learn more »
  
  </a>

  

  

  
  <div class="pro">
    <h5>PRO FEATURE</h5>
    <p>To add your logo to your survey, upgrade to a pro plan.</p>
    <p><a href="/pricing/upgrade/?ut_source=wall_logo&amp;ut_source2=ssum" class="btn btn-small yellow">Upgrade</a></p>
  </div>
  

  

</script>

<script id="upgrade-logic-popout-template" type="text/html">
  

  <h5>ADD LOGIC</h5>
  <p>You can create powerful surveys by adding logic including Question Skip Logic, Page Randomization, Question Randomization,	and more.</p>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/How-do-I-create-conditional-skip-logic?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">
  
    Learn more »
  
  </a>

  

  

  
  <div class="pro">
    <h5>PRO FEATURE</h5>
    <p>To add logic to your survey, upgrade to a pro plan.</p>
    <p><a href="/pricing/upgrade/?ut_source=wall_skiplogic&amp;ut_source2=ssum" class="btn btn-small yellow">Upgrade</a></p>
  </div>
  

  

</script>
        <script id="survey-summary-activity-template" type="text/html">
    <div class="primary">
        <div class="mod survey-activity-container">
            <header class="mod-header clearfix">
                <h3 class="sm-float-l txt-shadow-dark"><span class="all-caps">Response Summary</span></h3>
                <h3 class="sm-float-r txt-shadow-dark">
                    <span class="smf-icon q-on-dark">:</span>&nbsp;&nbsp;Survey Alerts:&nbsp;
                    <%# canEditSurveyAlerts %>
                      <%# surveyAlertsOn %>
                        <span class="alerts-on-off-link alerts-on2off-trigger">
                            <a href="#" alerts-on2off-trigger>On</a>
                        </span>
                      <%/ surveyAlertsOn %>
                      <%^ surveyAlertsOn %>
                        <span class="alerts-on-off-link alerts-off2on-trigger">
                            <a href="#" alerts-off2on-trigger>Off</a>
                        </span>
                      <%/ surveyAlertsOn %>
                    <%/ canEditSurveyAlerts %>
                    <%^ canEditSurveyAlerts %>
                      <%# surveyAlertsOn %>
                        <span>
                          On
                        </span>
                      <%/ surveyAlertsOn %>
                      <%^ surveyAlertsOn %>
                        <span>
                          Off
                        </span>
                      <%/ surveyAlertsOn %>
                    <%/ canEditSurveyAlerts %>
                </h3>
            </header>
            <div class="mod-body"></div>
        </div>
    </div>
</script>


<script id="responses-trend-header-template" type="text/html">
    <div class="clearfix spacer-pam">
        <div class="sm-float-r negative">
            <%start%> - <%end%>
        </div>
        <div class="sm-float-l responses-volume-text">
            Responses Volume
        </div>
    </div>
</script>

<script id="responses-trend-cta-template" type="text/html">
    <div class="clearfix spacer-pam responses-trend-cta-container">
        <a href="/analyze/<%encryptedID%>" class="btn btn-small">
            Analyze Results
        </a>
    </div>
</script>

<script id="survey-alerts-on2off-template" type="text/html">
    <ul class="option-menu">
      <li class="survey-alert-action-menu-option">
          <a class="option turn-on-off-alerts-link" data-action="a" href="/summary/notifications/opt-in-update/VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D/0">Turn off survey alerts</a>
          <div class="q">
            <span>?</span>
            <div class="popout">
              <h5>SURVEY ALERTS</h5>
              <p>Survey alerts let you know when your open surveys receive new responses. Alerts are emailed to you daily.</p>
              <a href="http://help.surveymonkey.com/articles/en_US/kb/Survey-Alerts?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link">Learn more &raquo;</a>
            </div>
          </div>
      </li>
    </ul>
</script>

<script id="survey-alerts-off2on-template" type="text/html">
    <ul class="option-menu">
      <li class="survey-alert-action-menu-option">
          <a class="option turn-on-off-alerts-link" data-action="a" href="/summary/notifications/opt-in-update/VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D/1">Turn on survey alerts</a>
          <div class="q">
            <span>?</span>
            <div class="popout">
              <h5>SURVEY ALERTS</h5>
              <p>Survey alerts let you know when your open surveys receive new responses. Alerts are emailed to you daily.</p>
              <a href="http://help.surveymonkey.com/articles/en_US/kb/Survey-Alerts?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link">Learn more &raquo;</a>
            </div>
          </div>
      </li>
    </ul>
</script>


        <script type="text/html" id="collector-list-template">
    <div class="collector-list">
        <%#hasCollectors%>
	        <div class="collectors-heading-text spacer-phm spacer-ptm spacer-pbs">
	            Collectors
	        </div>
        <%/hasCollectors%>
		<%^hasCollectors%>
			<div class="collector-item no-collectors-message">
			    <span class="negative">
			        No collectors added
			        <a no-collectors-help-link href="#" data-help="no-collectors-help-popout-template">
			            What is this?
			        </a>
			    </span>
			</div>
		<%/hasCollectors%>
	</div>
</script>

<script  type="text/html" id="collector-list-item-template">
  <div class="sm-grid collector-item <%#isDisabled%>disabled<%/isDisabled%>">
    <div class="sm-grid-block-row-start sm-grid-block collector-title sm-grid-block-40">
      <%^isDisabled%>
				<a class="collector-link clearfix" href="<%link%>">
			<%/isDisabled%>
			<%#isDisabled%>
				<span class="collector-link clearfix">
			<%/isDisabled%>
      <%#isLink%>
          <span class="icon smf-icon link-collector-icon">
               A
          </span>
      <%/isLink%>
      <%#isPopup%>
          <span class="icon smf-icon website-collector-icon">
               N
          </span>
      <%/isPopup%>
      <%#isFacebook%>
          <span class="icon smf-icon fb-collector-icon">
              Ñ
          </span>
      <%/isFacebook%>
      <%#isEmail%>
          <span class="icon smf-icon email-collector-icon">
               M
          </span>
      <%/isEmail%>
      <%#isAudience%>
          <span class="icon smf-icon audience-collector-icon">
               g
          </span>
      <%/isAudience%>
      <span class="collector-title">
          <%title%>
      </span>
      <%#showCollectorType%>
      <span class="collector-title">
          (<%formattedType%>)
      </span>
      <%/showCollectorType%>
      <%^isDisabled%>
	       </a>
			<%/isDisabled%>
			<%#isDisabled%>
				</span>
			<%/isDisabled%>
    </div>
    <div class="sm-grid-block sm-grid-block-20 collector-responses">
        Responses: <%formattedResponseCount%>
    </div>
    <%# dateCreated %>
        <div class="sm-grid-block sm-grid-block-20 collector-open-date">Since <%formattedDate%></div>
    <%/ dateCreated %>
    <div class="sm-grid-block sm-grid-block-20 collector-status">
 			<%^isDisabled%>
        <%#isOpen%>
            <a href="<%link%>" class="all-caps open-collector">Open</a>
        <%/isOpen%>
        <%#isClosed%>
            <a href="<%link%>" class="all-caps closed-collector">Closed</a>
        <%/isClosed%>
        <%#isUnconfigured%>
            <a href="<%link%>" class="all-caps unconfigured-collector">Not Configured</a>
        <%/isUnconfigured%>
        <%#isArchived%>
            <a href="<%link%>" class="all-caps archived-collector">Archived</a>
        <%/isArchived%>
 			<%/isDisabled%>
 			<%#isDisabled%>
        <%#isOpen%>
            <span class="all-caps open-collector">Open</span>
        <%/isOpen%>
        <%#isClosed%>
            <span class="all-caps closed-collector">Closed</span>
        <%/isClosed%>
        <%#isUnconfigured%>
            <span class="all-caps unconfigured-collector">Not Configured</span>
        <%/isUnconfigured%>
        <%#isArchived%>
            <span class="all-caps archived-collector">Archived</span>
        <%/isArchived%>
 			<%/isDisabled%>
      <%#isClearing%>
          <span class="all-caps closed-collector">Clearing...</span>
      <%/isClearing%>
    </div>
  </div>
</script>

<script id="no-collectors-help-popout-template" type="text/html">
  <h5>COLLECTORS</h5>
  <p>
    A collector is a method for sending out your survey
	to get responses. Collection methods include a web link,
	email, Facebook and others. Be sure to complete your survey
	design before creating a collector and collecting responses.
  </p>
   <div class="spacer-mbs">
	   <a href="/collect/list?sm=VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D" class="btn btn-small teal">
	        + Add a Collector
	   </a>
   </div>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/How-do-I-send-my-survey-to-respondents-or-get-responses-to-my-survey?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">Learn more »</a>
</script>
        <script type="text/html" id="respondent-stats-template">
    <div class="respondents-stats-container">
		<div class="sm-grid sm-grid-50">
		    <div class="sm-grid-block-row-start sm-grid-block">
		        <div class="activity-block">
			        <div class="activity-figures stat-count">
			            <%#hasResponses%>
				            <a href="/analyze/<%encryptedID%>" >
				                <% respondentContextTotal %>
				            </a>
				            <%#isOverResponseLimit%>
					            <a href="/analyze/<%encryptedID%>" class="respondent-stats-total-count">
					                <% respondentTotalCount %>
					            </a>
				            <%/isOverResponseLimit%>
			            <%/hasResponses%>
			            <%^hasResponses%>
			                <span class="no-responses-text txt-shadow-lt">0</span>
			            <%/hasResponses%>
			        </div>
			        <div class="activity-label">
			            <%#isOverResponseLimit%> Visible / <%/isOverResponseLimit%>Total Responses
			        </div>
		        </div>
		    </div>
		    <div class="sm-grid-block">
                <div class="activity-block activity-block-status">
			        <div class="activity-figures">
			            <%#isInDraft%>
			                <a href="/create/?sm=<%encryptedID%>" class="all-caps stat-count draft-survey">Draft</a>
			            <%/isInDraft%>
			            <%#isOpen%>
		                    <a href="/collect/list?sm=<%encryptedID%>" class="all-caps stat-count open-survey">Open</a>
		                    &nbsp;
		                    <%#isSurveyAlertsOn%>
	                            <span class="smf-icon q-on-dark alerts-indicator">:</span>
                            <%/isSurveyAlertsOn%>
			            <%/isOpen%>
			            <%#isClosed%>
		                    <a href="/collect/list?sm=<%encryptedID%>" class="all-caps stat-count closed-survey">Closed</a>
			            <%/isClosed%>
			            <%#isUnconfigured%>
		                    <a href="/collect/list?sm=<%encryptedID%>" class="all-caps stat-count draft-survey">Unconfigured</a>
			            <%/isUnconfigured%>
			        </div>
			        <div class="activity-label">
			            Overall Survey Status
			        </div>
		        </div>
		    </div>
		</div>
	</div>
</script>
        
<script type="text/html" id="no-trend-data-template">
		<div class="no-responses-message">
		    <span class="negative">
		        No survey responses
		        <a no-responses-help-link href="#" data-help="no-trend-data-help-popout-template">
		            What is this?
		        </a>
		    </span>
		</div>
</script>

<script id="no-trend-data-help-popout-template" type="text/html">
  

  <h5>DATA TRENDS CHART</h5>
  <p>The data trends chart shows you when you received responses to your survey.</p>
  <a href="http://help.surveymonkey.com/articles/en_US/kb/Data-Trends?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" class="learn-more-link" target="_blank">
  
    Learn more »
  
  </a>

  

  

  

  

</script>
        <script type="text/html" id="survey-steps-template">
    <table class="survey-steps-container spacer-mbx <%^inStep2or3%> even-distribute <%/inStep2or3%>">
        <tbody>
            <tr>
                <td>
                    <%#afterStep2%>
                        <a href="/create/?sm=<%encryptedID%>" class="survey-step survey-step-first completed">
                    <%/afterStep2%>
                    <%#beforeStep3%>
                        <div class="survey-step survey-step-first selected">
                    <%/beforeStep3%>
                            <div class="inner-survey-step sm-corner-l clearfix">
                                <h5>
                                    <%#inStep1%>
                                        1. Design your survey
                                    <%/inStep1%>
                                    <%#afterStep1%>
                                        1. Edit your survey
                                    <%/afterStep1%>
                                </h5>
                                <%#inStep1%>
                                    <a href="/create/?sm=<%encryptedID%>" class="btn teal sm-float-r">
                                        + Add Questions
                                    </a>
                                <%/inStep1%>
                            </div>
                            <div class="survey-step-pointer"></div>
                    <%#afterStep2%>
                        </a>
                    <%/afterStep2%>
                    <%#beforeStep3%>
                        </div>
                    <%/beforeStep3%>
                </td>
                <td>
                    <%#inStep4%>
                        <a href="/collect/list?sm=<%encryptedID%>" class="survey-step completed">
                    <%/inStep4%>
                    <%#beforeStep4%>
                        <div class="survey-step <%#inStep3%>selected<%/inStep3%>">
                    <%/beforeStep4%>
                            <div class="survey-step-tail"></div>
                            <div class="inner-survey-step clearfix">
                                <h5>2. Collect survey responses</h5>
                                <%#inStep3%>
                                    <div class="sm-float-r survey-step-btns">
                                        <a href="/collect/list?sm=<%encryptedID%>" class="btn teal">
                                            <%#hasOpenCollector%>
                                                Go to Collect
                                            <%/hasOpenCollector%>
                                            <%^hasOpenCollector%>
                                                Edit Collectors
                                            <%/hasOpenCollector%>
                                        </a>
                                        <%#shouldShowBuyResponsesButton%>
                                            <h5 class="or">or</h5>
                                            <a href="/collect/audience/getstarted/?ut_source=sma&ut_source2=li_survey_summary&survey_id=<%surveyID%>" class="btn yellow">
                                                Buy Responses
                                            </a>
                                        <%/shouldShowBuyResponsesButton%>
                                    </div>
                                <%/inStep3%>
                                <%#inStep2%>
                                    <div class="sm-float-r survey-step-btns">
                                        <a href="/collect/list?sm=<%encryptedID%>" class="btn teal">
                                            <%^hasCollectors%>+ Add a Collector<%/hasCollectors%>
                                        </a>
                                    </div>
                                <%/inStep2%>
                            </div>
                            <div class="survey-step-pointer"></div>
                    <%#inStep4%>
                        </a>
                    <%/inStep4%>
                    <%#beforeStep4%>
                        </div>
                    <%/beforeStep4%>
                </td>
                <td>
                    <div class="survey-step survey-step-last <%#inStep4%> selected <%/inStep4%>">
                        <div class="survey-step-tail"></div>
                        <div class="inner-survey-step sm-corner-r clearfix">
                            <h5>3. Analyze your results</h5>
                            <%#inStep4%>
                                <a href="/analyze/<%encryptedID%>" class="btn teal sm-float-r">
                                    Go to Analyze
                                </a>
                            <%/inStep4%>
                        </div>
                    </div>
                </td>
            </tr>
        </tbody>
    </table>
</script>
        <script type="text/html" id="ltdl-container-template">
    <div class="ltdl-container">
    </div>
</script>

<script type="text/html" id="highcharts-trend-chart-template">
    <div class="highcharts-chart-container highcharts-trend-chart-container"></div>
</script>

<script type="text/html" id="ltdl-page-list-template">
    <div class="sm-analyze-pages">
    </div>
</script>

<script type="text/html" id="ltdl-page-template">
    <div analyze-mode-content sm-analyze-page class="sm-analyze-page fadeable" sm-page-id="<%id%>">
    </div>
</script>

<script type="text/html" id="ltdl-page-title-template">
    <div class="page-header sm-corner-t <%^isVisible%>hidden<%/isVisible%>">
        <span class="page-title">PAGE <%number%><%#title%>: <%title%> <%/title%></span>
    </div>
</script>


<script type="text/html" id="ltdl-question-list-template">
    <div></div>
</script>

<script type="text/html" id="ltdl-ttip-template">
    <%#isNPS%>
        <span style="font-weight: bold;">NPS: <%score%></span>
        <br><span class="sl_plural"><%total%></span> <%plural%>
    <%/isNPS%>
    <%^isNPS%>
        <%#showPercent%><%dataPointValue%> (<%percentage%>)<%/showPercent%>
        <%^showPercent%><span class="sl_plural"><%dataPointValue%></span> <%plural%><%/showPercent%>
    <%/isNPS%>
    <br><%time%>
</script>
<script type="text/html" id="ltdl-question-template">
    <div sm-question-view="" class="sm-question-view sm-corner-a <%^isVisible%>hidden<%/isVisible%>"
         sm-question-id="<%q.ID%>">
        <div sm-question-view-header class="sm-question-view-header clearfix">
            <span class="sm-question-number txt-shadow-lt heavy">
                Q<%q.position%>
            </span>
            <span class="sm-parenthetical txt-shadow-lt heavy">
                <%#trendBy.hour%>(by hour)<%/trendBy.hour%>
                <%#trendBy.day%>(by day)<%/trendBy.day%>
                <%#trendBy.week%>(by week)<%/trendBy.week%>
                <%#trendBy.month%>(by month)<%/trendBy.month%>
                <%#trendBy.quarter%>(by quarter)<%/trendBy.quarter%>
                <%#trendBy.year%>(by year)<%/trendBy.year%>
            </span>
            <%^noMenu%>

            <div class="sm-question-btns clearfix">
                <div class="btn-menu sm-float-r sm-display-options">
                    <a href="#" trend-opts-btn=""
                       class="btn btn-menu-left btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Trend
                        by...<span></span></a>
                    <a href="#" zoom-opts-btn=""
                       class="btn btn-menu-right btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Zoom<span></span></a>
                </div>
                <div class="btn-menu sm-float-r sm-display-options<">
                    <a href="#" chart-opts-btn
                       class="btn btn-menu-left btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Chart
                        Type<span></span></a>
                    <a href="#" display-opts-btn
                       class="btn btn-menu-right btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Display
                        Options<span></span></a>
                </div>
            </div>
            <%/noMenu%>
        </div>

        <div sm-question-content="" class="sm-questionview-content">
            <h1 class="heavy sm-questiontitle">
                <%&q.heading%>
            </h1>
            <%^isNoData%>
            <%^isDisabledQuestionType%>
            <ul class="sm-question-view-sub-header heavy <%^isMultiCharts%>spacer-pbn<%/isMultiCharts%>">
                <li>
                    Answered: <%answered%>
                </li>
                <li>
                    Skipped: <%skipped%>
                </li>
                <li>
                    First: <%startDate%>
                </li>
                <li class="sm-zoom-text">
                    Zoom: <%zoomStartDate%> to <%zoomEndDate%>
                </li>
            </ul>
            <%/isDisabledQuestionType%>
            <%#isDisabledQuestionType%>
            <h3 class="sm-question-view-disabled-txt txt-grymeddrk">
                <%disabledMsg%>
            </h3>
            <%/isDisabledQuestionType%>
            <div class="sm-chart-container"></div>
            <%/isNoData%>
            <%#isNoData%>
            <h3 class="sm-question-view-disabled-txt txt-grymeddrk">
                <%noDataMsg%>
            </h3>
            <%/isNoData%>
        </div>
    </div>
</script>

<script type="text/html" id="ltdl-zoom-window-template">
    <div>
        Zoom: <%zoomStartDate%> to <%zoomEndDate%>
    </div>
</script>

<script type="text/html" id="ltdl-responses-template">
    <div class="sm-responses-view <%^show%>sm-responses-hide<%/show%>">
        <div class="sm-question-view sm-corner-a">
            <div sm-question-view-header class="sm-question-view-header clearfix">
                <span class="sm-question-number txt-shadow-lt heavy">
                    <%#hour%>Responses (by hour)<%/hour%>
                    <%#day%>Responses (by day)<%/day%>
                    <%#week%>Responses (by week)<%/week%>
                    <%#quarter%>Responses (by quarter)<%/quarter%>
                    <%#month%>Responses (by month)<%/month%>
                    <%#year%>Responses (by year)<%/year%>
                </span>
                <div class="sm-question-btns clearfix">
                    <div class="btn-menu sm-float-r sm-display-options">
                        <a href="#" trend-opts-btn=""
                           class="btn btn-menu-left btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Trend by... <span></span></a>
                        <a href="#" zoom-opts-btn=""
                           class="btn btn-menu-right btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow"> Zoom <span></span></a>
                    </div>
                    <div class="btn-menu sm-float-r sm-display-options<">
                        <a href="#" chart-opts-btn
                           class="btn btn-small btn-arrow btn-arrow-right btn-arrow-small-vert btn-arrow-small-down-dark grey btn-txt-secondary no-shadow">Chart Type<span></span></a>
                    </div>
                </div>
            </div>
            <div class="sm-questionview-content">
                <%^isNoData%>
                <ul class="sm-question-view-sub-header heavy spacer-pbn spacer-ptx">
                    <li>
                        First: <%startDate%>
                    </li>
                    <li class="sm-zoom-text">
                        Zoom: <%zoomStartDate%> to <%zoomEndDate%>
                    </li>
                </ul>
                <div class="sm-chart-container"></div>
                <%/isNoData%>
                <%#isNoData%>
                <h3 class="sm-question-view-disabled-txt txt-grymeddrk">
                    <%noDataMsg%>
                </h3>
                <%/isNoData%>
            </div>
        </div>
    </div>
</script>
<script type="text/html" id="global-all-chart-menu-template">
    <ul class="option-menu">
        <li class="sm-menu-chart-container">
            <ol class="sm-chart-menu">
                <li class="stacked_vbar" title="Stacked Vertical Bar">
                    <a class="option <%^stacked_vbar.isEnabled%>disabled<%/stacked_vbar.isEnabled%> <%#stacked_vbar.isSelected%>selected<%/stacked_vbar.isSelected%>"
                       data-action="stacked_vbar" href="#">
                        Stacked Vertical Bar
                    </a>
                </li>
                <li class="vbar" title="Vertical Bar">
                    <a class="option <%^vbar.isEnabled%>disabled<%/vbar.isEnabled%> <%#vbar.isSelected%>selected<%/vbar.isSelected%>"
                       data-action="vbar" href="#">
                        Vertical Bar
                    </a>
                </li>
                <li class="area" title="Area Graph">
                    <a class="option <%^area.isEnabled%>disabled<%/area.isEnabled%> <%#area.isSelected%>selected<%/area.isSelected%>"
                       data-action="area" href="#">
                        Area Graph
                    </a>
                </li>
                <li class="line" title="Line Graph">
                    <a class="option <%^line.isEnabled%>disabled<%/line.isEnabled%> <%#line.isSelected%>selected<%/line.isSelected%>"
                       data-action="line" href="#">
                        Line Graph
                    </a>
                </li>
            </ol>
        </li>
    </ul>
</script>

<script type="text/html" id="trend-by-menu-template">
    <ul class="option-menu trend-by-menu">
        <li class="test <%^hour.visible%>hidden<%/hour.visible%>">
            <a class="option <%#hour.disabled%>disabled<%/hour.disabled%> <%#hour.selected%>selected<%/hour.selected%>"
               data-action="hour" href="#">Hours</a>
        </li>
        <li class="<%^day.visible%>hidden<%/day.visible%>">
            <a class="option <%#day.disabled%>disabled<%/day.disabled%> <%#day.selected%>selected<%/day.selected%>"
               data-action="day" href="#">Days</a>
        </li>
        <li class="<%^week.visible%>hidden<%/week.visible%>">
            <a class="option <%#week.disabled%>disabled<%/week.disabled%> <%#week.selected%>selected<%/week.selected%>"
               data-action="week" href="#">Weeks</a>
        </li>
        <li class="<%^month.visible%>hidden<%/month.visible%>">
            <a class="option <%#month.disabled%>disabled<%/month.disabled%> <%#month.selected%>selected<%/month.selected%>"
               data-action="month" href="#">Months</a>
        </li>
        <li class="<%^quarter.visible%>hidden<%/quarter.visible%>">
            <a class="option <%#quarter.disabled%>disabled<%/quarter.disabled%> <%#quarter.selected%>selected<%/quarter.selected%>"
               data-action="quarter" href="#">Quarters</a>
        </li>
        <li class="<%^year.visible%>hidden<%/year.visible%>">
            <a class="option <%#year.disabled%>disabled<%/year.disabled%> <%#year.selected%>selected<%/year.selected%>"
               data-action="year" href="#">Years</a>
        </li>
    </ul>
</script>

<script type="text/html" id="zoom-menu-template">
    <ul class="option-menu">
        <li class="<%^day.visible%>hidden<%/day.visible%>">
            <a class="option <%#day.selected%>selected<%/day.selected%>" data-action="day" href="#"><span class="sl_plural">24</span> hours</a>
        </li>
        <li class="<%^week.visible%>hidden<%/week.visible%>">
            <a class="option <%#week.selected%>selected<%/week.selected%>" data-action="week" href="#"><span class="sl_plural">7</span> days</a>
        </li>
        <li class="<%^month.visible%>hidden<%/month.visible%>">
            <a class="option <%#month.selected%>selected<%/month.selected%>" data-action="month" href="#"><span class="sl_plural">30</span> days</a>
        </li>
        <li class="<%^quarter.visible%>hidden<%/quarter.visible%>">
            <a class="option <%#quarter.selected%>selected<%/quarter.selected%>" data-action="quarter" href="#"><span class="sl_plural">3</span> months</a>
        </li>
        <li class="<%^year.visible%>hidden<%/year.visible%>">
            <a class="option <%#year.selected%>selected<%/year.selected%>" data-action="year" href="#"><span class="sl_plural">12</span> months</a>
        </li>
        <li class="<%^three_years.visible%>hidden<%/three_years.visible%>">
            <a class="option <%#three_years.selected%>selected<%/three_years.selected%>" data-action="three_years"
               href="#"><span class="sl_plural">3</span> years</a>
        </li>
        <li class="<%^max.visible%>hidden<%/max.visible%>">
            <a class="option <%#max.selected%>selected<%/max.selected%>" data-action="max" href="#">Max</a>
        </li>
    </ul>
</script>

<script type="text/html" id="chart-opts-menu-template">
    <ul class="option-menu trend-chart-menu">
        <li class="sm-menu-chart-container">
            <ol class="sm-chart-menu">
                <li class="vbar" title="Column Chart">
                    <a class="option <%^column.enabled%>disabled<%/column.enabled%> <%#column.selected%>selected<%/column.selected%>"
                       data-action="column" href="#">
                        Column Chart
                    </a>
                </li>
                <li class="area" title="Area Chart">
                    <a class="option <%^area.enabled%>disabled<%/area.enabled%> <%#area.selected%>selected<%/area.selected%>"
                       data-action="area" href="#">
                        Area Chart
                    </a>
                </li>
                <li class="line" title="Line Chart">
                    <a class="option <%^line.enabled%>disabled<%/line.enabled%> <%#line.selected%>selected<%/line.selected%>"
                       data-action="line" href="#">
                        Line Chart
                    </a>
                </li>
            </ol>
        </li>
    </ul>
</script>

<script type="text/html" id="display-opts-menu-template">
    <ul class="option-menu trend-display-menu">
        <%#isChartShown%>
        <%#showPercent%>
        <li class="hide-chart">
            <a class="option" data-action="showValue" href="#">Switch axis to absolute</a>
        </li>
        <%/showPercent%>
        <%^showPercent%>
        <li class="hide-chart">
            <a class="option <%#disableShowPercentage%>disabled<%/disableShowPercentage%> " data-action="showPercent"
               href="#">Switch axis to percentage</a>
        </li>
        <%/showPercent%>
        <%/isChartShown%>
        <%^isChartShown%>
        <li class="hide-chart">
            <a class="option disabled" data-action="showPercent" href="#">Switch axis to percentage</a>
        </li>
        <%/isChartShown%>
    </ul>
</script>


<script type="text/html" id="trend-chart-display-error-template">
    <div class="sm-chart-error">
        <span class="smf-icon">!</span> Oops!, something went wrong displaying your trend chart.
    </div>
</script>
        <!-- upgrade dialogs -->

<script type="text/html" id="rules-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="rules_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Upgrade to use Saved Views" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Dig Into Your Data</h1>

                <h2>Start slicing and dicing.</h2>

                <p> Upgrade to understand what your data is really telling you. With crosstabs and filters,
                    you compare questions side by side and filter by response, collector, and more. </p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_rulelimit&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="saved-views-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="saved_views_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Upgrade to use saved views" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>See Data in Multiple Ways</h1>

                <h2>Save your filters and views.</h2>

                <p>Upgrade to create and save multiple views of your survey data based on different
                combinations of filters and crosstabs.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_savedview&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="export-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="export_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div class="upgrade-dialog-graphic"></div>
            </div>
            <div class="upgrade-dialog-text">
                <h1>Put Your Data to Work</h1>

                <h2>Export in the formats you want.</h2>

                <p>Upgrade to export your survey results as PowerPoints, spreadsheets, and more.
                    Download your data into any of these formats: CSV, PNG, PDF, PPT, SPSS and XLS.</p>
            </div>
        </div>
        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_exporting&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="export-single-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="export_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div class="upgrade-dialog-graphic"></div>
            </div>
            <div class="upgrade-dialog-text">
                <h1>Put Your Data to Work</h1>

                <h2>Export in the formats you want.</h2>

                <p>Upgrade to export your survey results as PowerPoints, spreadsheets, and more.
                    Download your data into any of these formats: CSV, PNG, PDF, PPT, SPSS and XLS.</p>
            </div>
        </div>
        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_export_question&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="export-chart-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="export_chart_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div class="upgrade-dialog-graphic"></div>
            </div>
            <div class="upgrade-dialog-text">
                <h1>Show Off Your Results</h1>

                <h2>Use your charts anywhere.</h2>

                <p>Make your data pop by using your charts in print, presentations, or by posting them online.
                    Upgrade to download charts as a PNG or to export data in other formats.</p>
            </div>
        </div>
        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_export_chart&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="manage-responses-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="manage_responses_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Sick of Taking Out the Trash?</h1>

                <h2>Easily manage responses.</h2>

                <p>You&#39;ve just deleted your 50th respondent. Upgrade today to delete more responses—and also filter
                    and compare responses, so you can see everything your data is telling you.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=delete_limit&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="trends-upgrade-dialog-template">
    <div class="dialog upgrade-dialog trends-upgrade-dialog" id="trends_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Upgrade to use Data Trends" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>See Trends in Your Data</h1>

                <h2>Track your results over time.</h2>

                <p>Upgrade to compare answers by time period. Get deeper insights by seeing how responses to the same questions change over time.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_data_trends&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="customize-upgrade-dialog-template">
    <div class="dialog upgrade-dialog customize-upgrade-dialog" id="customize_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Upgrade to customize colors" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Let Your Brand Shine</h1>

                <h2>Customize your colors.</h2>

                <p>Upgrade to change colors in your charts to match your brand identity. Make single-color charts,
                    use shades to emphasize differences, and easily apply colors to all your charts.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_chartcust_colors&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="password-sharing-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="password_sharing_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Password Protection" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Add Password Protection</h1>

                <h2>Protect your shared data.</h2>

                <p>Upgrade to add an extra layer of protection to survey data you choose to share, so only people with a password
                    can view it. Plus, get more ways to analyze your data with filters, crosstabs and more.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_password_sharing&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="hide-logo-sharing-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="hide_logo_sharing_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Power Sharing" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Be the Only Brand They See</h1>

                <h2>Hide our logo.</h2>

                <p>Upgrade to hide the SurveyMonkey logo on your shared data page. Available with GOLD, and PLATINUM plans.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_sharing&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<!-- upgrade messages -->

<script type="text/html" id="upgrade-response-limit-template">
    <div class="upgrade-message <%classes%> clearfix" id="response_limit_upgrade_message">
        <span class="smf-icon">!</span>

        <p class="upgrade-description">
            <span class="upgrade-title">Maximum Response Limit:</span>
            You have reached your limit of <%responseLimit%> survey responses. To see all <%responseCount%> responses,
            upgrade to any pro plan.
        </p>

        <a class="btn yellow upgrade-btn btn-small" href="/pricing/upgrade/?ut_source=<%linkSource%>">Upgrade</a>
    </div>
</script>

<script type="text/html" id="export-upgrade-message-template">
    <div class="upgrade-message sm-corner-a" id="export_upgrade_message">
        <h6 class="upgrade-title">PRO FEATURE</h6>

        <p class="upgrade-description">
            Export your survey data in .PDF, .XLS, .CSV, .PPTX, or SPSS format.
        </p>

        <a class="btn btn-small yellow upgrade-btn space-mrs"
            href="/pricing/upgrade/?ut_source=wall_exporting&ut_source2=new_analyze">
            Upgrade
        </a>
        <a learn-more class="learn-more" href="#">Learn more &raquo;</a>
    </div>
</script>

<script type="text/html" id="rule-limit-upgrade-message-template">
    <div class="upgrade-message sm-corner-a" id="rule_limit_upgrade_message">
        <h6 class="upgrade-title">PRO FEATURE</h6>

        <p class="upgrade-description">
            Create unlimited rules (FILTER, COMPARE, and SHOW) to dive even deeper into your data.
        </p>
        <a class="btn btn-small yellow upgrade-btn space-mrs" href="/pricing/upgrade/?ut_source=wall_rulelimit&ut_source2=new_analyze">
            Upgrade
        </a>
        <a class="learn-more" href="#">Learn more &raquo;</a>
    </div>
</script>

        <script type="text/html" id="white-label-sharing-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="white_label_sharing_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="White Label Sharing" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Be the Only Brand They See</h1>

                <h2>White label your shared data.</h2>

                <p>Upgrade to a PLATINUM plan to publish your surveys and shared data on research.net.
                    You&#39;ll also be able to remove SurveyMonkey branding.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_sharing&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="sig-diff-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="sig_diff_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div title="Statistical Significance" class="upgrade-dialog-graphic"></div>
            </div>

            <div class="upgrade-dialog-text">
                <h1>Be Confident in Your Results</h1>

                <h2>See statistical significance.</h2>

                <p>Upgrade to see statistical significance for your responses and get more ways to analyze your data. Available with GOLD and PLATINUM plans.</p>
            </div>
        </div>

        <div class="dialog-btn-bar clearfix">
            <a class="btn yellow upgrade-btn" href="/pricing/upgrade/?ut_source=wall_sig_difs&ut_source2=new_analyze">Upgrade</a>
            <a class="btn cancel-btn dialog-close-btn" href="#">No thanks</a>
        </div>
    </div>
</script>

<script type="text/html" id="export-hide-branding-upgrade-dialog-template">
    <div class="dialog upgrade-dialog" id="export_hide_branding_upgrade_dialog">
        <div class="upgrade-dialog-content clearfix">
            <div class="upgrade-dialog-graphic-container">
                <div class="upgrade-dialog-graphic"></div>
            </div>
            <div class="upgrade-dialog-text">
                <h1>Take All the Credit</h1>

                <h2>Hide our branding.</h2>

                <p>Upgrade to hide SurveyMonkey branding in your presentations. Available with GOLD or PLATINUM plans.</p>
            </div>
        </div>
        <div class="dialog-btn-bar clearfix">
            <a href="/pricing/upgrade/?ut_source=wall_export_hidebrand&ut_source2=new_analyze" class="upgrade-btn btn yellow">Upgrade</a>
            <a href="#" class="cancel-btn btn dialog-close-btn">No thanks</a>
        </div>
    </div>
</script>

        
        <script id="ucs-content-modules-template" type="text/html">
    <div class="ucs-content-modules-container secondary">
        
            <div id="ucs-survey-summary-benchmarks" class="mod">
    <header class="mod-header clearfix">
        <h3 class="sm-float-l txt-shadow-dark">
            SEE HOW YOUR RESULTS STACK UP
        </h3>
    </header>
    <div class="mod-body">
        <p>Use benchmarks to see how your results compare to industry leaders and get the context you need to:</p>
        <ul>
            <li>Assess performance metrics more accurately</li>
            <li>Set realistic goals</li>
            <li>Make targeted improvements</li>
        </ul>
        <div class="ucs-img-wrapper">
            <a href="/mp/why-use-benchmarks/?ut_source=ssum&ut_source2=benchmarks">
                <img class="ucs-benchmarks-img" src="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc/0.0.0.113/assets/benchmarks_no_qb_qus.png">
            </a>
        </div>
    </div>
    <div class="module-footer">
        <a href="/mp/why-use-benchmarks/?ut_source=ssum&ut_source2=benchmarks" class="btn btn-small">Learn More</a>
    </div>
</div>
        
    </div>
</script>
    </div>

                </div>
            </div>

            <div class="footer-push"></div>
        </div>

        
            


<div class="base-footer  auth-footer " id="ft">
    <div class="inner-ft">
        
            <div class="ft-c">
                <ul class="link-list">
                    <li id="FB_lnk_4" class="link-list-label SL_swap">
                        <a  href="http://www.facebook.com/pages/SurveyMonkey/65225997627" target="_blank" >
                            Community:
                        </a>
                    </li>
                    <li>
                        <a href="https://developer.surveymonkey.com" target="_blank">
                            Developers
                        </a>
                    </li>
                    <li id="FB_lnk_5" class="SL_swap">
                        <a  href="http://www.facebook.com/pages/SurveyMonkey/65225997627" target="_blank" title="Follow us on Facebook" >
                            Facebook
                        </a>
                    </li>
                    <li id="Twitter_lnk_3" class="SL_swap">
                        <a href="http://twitter.com/#!/SurveyMonkey" target="_blank" title="Follow us on Twitter" >
                            Twitter
                        </a>
                    </li>
                    <li>
                        <a href="http://www.linkedin.com/company/362798" target="_blank" title="Follow us on LinkedIn">
                            LinkedIn
                        </a>
                    </li>
                    <li id="Intl_blog_1" class="SL_swap">
                        <a href="http://www.surveymonkey.com/blog/en/" target="_blank" title="Subscribe to our blog">
                            Our Blog
                        </a>
                    </li>
                    <li id="footer_gplus" class="google-plus SL_swap">
                        <a href="https://plus.google.com/+surveymonkey/posts" target="_blank" title="Follow us on Google +">
                            Google+
                        </a>
                    </li>
                    <li>
                        <a href="http://www.youtube.com/surveymonkey" target="_blank" title="Follow us on YouTube">
                            YouTube
                        </a>
                    </li>
                </ul>
                <ul class="link-list">
                    <li class="link-list-label">
                        <a href="/mp/aboutus/">
                            About Us:
                        </a>
                    </li>
                    <li>
                        <a href="/mp/aboutus/management/">
                            Management Team
                        </a>
                    </li>
                     <li>
                        <a href="/mp/aboutus/directors/">
                            Board of Directors
                        </a>
                    </li>
                    <li>
                        <a href="/integrations/">
                            Integrations
                        </a>
                    </li>
                    <li>
                        <a href="/mp/aboutus/newsroom/">
                            Newsroom
                        </a>
                    </li>
                    <li>
                        <a href="/mp/aboutus/office-locations/">
                            Office Locations
                        </a>
                    </li>
                    
                    
                    <li id="Jobs_1" class="SL_swap">
                        <a href="/mp/jobs/" target="_blank">
                            Jobs
                        </a>
                    </li>
                    <li>
                        <a href="/mp/sitemap/">
                            Sitemap
                        </a>
                    </li>
                    <li>
                        <a href="http://help.surveymonkey.com/?l=en_US&amp;uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" target="_blank">
                            Help
                        </a>
                    </li>
                </ul>
                <ul class="link-list">
                    <li class="link-list-label">
                        <a href="/mp/policy/">
                            Policies:
                        </a>
                    </li>
                    <li>
                        <a href="/mp/policy/terms-of-use/">
                            Terms of Use
                        </a>
                    </li>
                    <li>
                        <a href="/mp/policy/privacy-policy/">
                            Privacy Policy
                        </a>
                    </li>
                    <li>
                        <a href="/mp/policy/anti-spam/">
                            Anti-Spam Policy
                        </a>
                    </li>
                    <li>
                        <a href="/mp/policy/security/">
                            Security Statement
                        </a>
                    </li>
                    <li>
                        <a href="/optin.aspx">
                            Email Opt-In
                        </a>
                    </li>
                    <li>
                        <a href="http://help.surveymonkey.com/articles/en_US/kb/508-Compliance?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D">
                            Accessibility
                        </a>
                    </li>
                </ul>
            </div>
            <div class="ft-c lang-list clearfix">
                <i class="smf-icon world-icon">°</i>
                

                <ul class="link-list">
                    <li class="link-list-label">
                        Language:
                    </li>
                    
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=1"
                                   class="selected">English</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=19"
                                   class="">Español</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=16"
                                   class="">Português</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=8"
                                   class="">Deutsch</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=5"
                                   class="">Nederlands</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=7"
                                   class="">Français</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=18"
                                   class="">Русский</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=10"
                                   class="">Italiano</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=4"
                                   class="">Dansk</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=20"
                                   class="">Svenska</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=11"
                                   class="">日本語</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=12"
                                   class="">한국어</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=3"
                                   class="">中文(繁體)</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=21"
                                   class="">Türkçe</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=14"
                                   class="">Norsk</a>
                            </li>
                            <li class="SL_opaque">
                                <a href="//www.surveymonkey.com/user/language?languageid=6"
                                   class="">Suomi</a>
                            </li>
                    
                </ul>
            </div>
        
        <div class="grid ft-bottom">
            <div class="col grid-u-2-5">
                
                <span class="copy">
                    Copyright &copy; 1999-2016 SurveyMonkey
                </span>
            </div>
            <div class="col grid-u-3-5">
                
                <ul class="security">
    <li>
        <a href="//privacy.truste.com/privacy-seal/validation?rid=923f19c3-37fc-49b9-871b-caae4c6840b3" class="link-truste" title="TRUSTe Privacy Certification" target="_blank">
          <img style="border: none" src="//privacy-policy.truste.com/privacy-seal/seal?rid=923f19c3-37fc-49b9-871b-caae4c6840b3" alt="TRUSTe Privacy Certification"/>
        </a>
    </li>
    <li>
        <a href="http://www.bbb.org/oregon/business-reviews/market-survey-companies/surveymonkeycom-in-portland-or-22010900" target="_blank" class="link-bbonline"  title="Click to verify BBB accreditation and to see a BBB report.">
            BBOnline
        </a>
    </li>
    <li>
        <a target="_blank" href="http://help.surveymonkey.com/articles/en_US/kb/508-Compliance?uid=_2FWewvtuB2x8V0ac_2BFozEArgu46q0_2FuYaIQyphTGF1C3bjD_2FZTS7T1ibZ3oVJIMF835E2appS3zsnNyRQ0b83MKKoV24IFB6VdN5dmmcANZc_3D" title="Equal Entry Accessibility Certification" class="link-equalentry" id="footer_hlRamp">
            Equal Entry
        </a>
    </li>
    










    
    
        
        
    




<li>
    <div id="DigiCertClickID_MUQGEFO_" data-language="en"></div>
    <script type="text/javascript">
    var __dcid = __dcid || [];__dcid.push(["DigiCertClickID_MUQGEFO_", "10", "s", "black", "MUQGEFO_"]);(function(){var cid=document.createElement("script");cid.async=true;cid.src="//seal.digicert.com/seals/cascade/seal.min.js";var s = document.getElementsByTagName("script");var ls = s[(s.length - 1)];ls.parentNode.insertBefore(cid, ls.nextSibling);}());
    </script>
</li>

    <li>
        <a href="https://seal.qualys.com/sealserv/info/?i=4b518e16-57ea-4f06-b68d-ee6b65604a47" target="_blank" class="link-qualys">
            Qualys
        </a>
    </li>
</ul>
            </div>
        </div>
    </div>
</div>
        

        
            <a href="/create/?ut_source=create_survey&ut_source2=bottomfab" class="create-survey fab lower-fab" title="Create Survey">
                <div class="vertical-line"></div>
                <div class="horizontal-line"></div>
            </a>
        

        

        <div class="hidden hidden-objects">
            
        </div>

        

        
            <script src="https://secure.surveymonkey.com/smassets/anweb/smlib.ui-global-bundle-min.5d45188f.js" 
    ></script>
        

        <script src="https://secure.surveymonkey.com/smassets/anweb/smlib.globaltemplates-base-bundle-min.d2f07182.js" 
    ></script>
        

        
            
                <script src="https://secure.surveymonkey.com/smassets/usercontentsvc/usercontentsvc-autorenew-bundle-min.e802a7c1.js"></script>
            
        

        

    

    <script src="https://secure.surveymonkey.com/smassets/anweb/smlib.ui-global-pro-bundle-min.d392c439.js" 
    ></script>
    <script src="https://secure.surveymonkey.com/smassets/anweb/anweb-survey-summary-bundle-min.741e4273.js" 
    ></script>
    <script type="text/javascript">
(function () {
    var translation,
            culture,
            serverTranslations;

    SM.translations = {};

    // -------------------------------------- Common Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Saved Views": "Saved Views",
        "Saved View": "Saved View",
        "Original View": "Original View",
        "File Name": "File Name",
        "Email Notification": "Email Notification",
        "Question": "Question",
        "Page": "Page",
        "Response time": "Response time",
        "complete responses": "complete responses",
        "partial responses": "partial responses",
        "disqualified responses": "disqualified responses",
        "responses over quota": "responses over quota",
        "Responses": "Responses",
        "Answer Choices": "Answer Choices",
        "Text Analysis": "Text Analysis",
        "My Categories": "My Categories",
        "Average Number": "Average Number",
        "Total Number": "Total Number",
        "Total": "Total",
        "Total Respondents": "Total Respondents",
        "Score": "Score",
        "Weighted Average": "Weighted Average",
        "Answer Choices": "Answer Choices",
        "Over a year": "Over a year",
        "Over a month": "Over a month",
        "Over a week": "Over a week",
        "Over a day": "Over a day",
        "Apply": "Apply",
        "Save": "Save",
        "Uncategorized": "Uncategorized",
        "Hide": "Hide",
        "Expand": "Expand",
        "edited": "edited",
        "no label": "no label",
        "All": "All",
        "COPY": "COPY",
        "Compare rules do not apply to this question": "Compare rules do not apply to this question",
        "filter": "filter",
        "show": "show",
        "compare": "compare",
        "hour": "hour",
        "minute": "minute",
        "second": "second",
        "Chart": "Chart",
        "Data": "Data",
        "All": "All",
        "Responses": "Responses",
        "Response": "Response",
        "New version available!": "New version available!",
        "Fresher bananas are available, let us reload this page for you...": "Fresher bananas are available, let us reload this page for you...",
        "No responses for this question": "No responses for this question",
        "Targeted Audience": "Targeted Audience",
        "Web Link": "Web Link",
        "Email": "Email",
        "Website Survey": "Website Survey",
        "Facebook Link": "Facebook Link",
        "Segment": "Segment",
        "Minimum": "Minimum",
        "Mean": "Mean",
        "Standard Deviation": "Standard Deviation",
        "Lower Quartile": "Lower Quartile",
        "Median": "Median",
        "Upper Quartile": "Upper Quartile",
        "Maximum": "Maximum",
        "Show Benchmarks": "Show Benchmarks",
        "Show Summary": "Show Summary",
        "Your score": "Your score",
        "Your average": "Your average",
        "Organizations": "Organizations",
        "Net Promoter Score": "Net Promoter Score",
        "Net Promoter&#174; Score": "Net Promoter&#174; Score",
        "Detractors": "Detractors",
        "Passives": "Passives",
        "Promoters": "Promoters",
        "Detractor": "Detractor",
        "Passive": "Passive",
        "Promoter": "Promoter",
        "Detractors (0-6)": "Detractors (0-6)",
        "Passives (7-8)": "Passives (7-8)",
        "Promoters (9-10)": "Promoters (9-10)",
        "Your Responses": "Your Responses",
        "Your Net Promoter&#174; Score": "Your Net Promoter&#174; Score",
        "Top 25%, " : "Top 25%, ",
        "Top 10%, " : "Top 10%, ",
        "Fetch Benchmark data failed": "Fetch Benchmark data failed",
        "We were unable to retrieve the benchmark data at this time. Please try again later.": "We were unable to retrieve the benchmark data at this time. Please try again later.",
        "Save New Segment failed": "Save New Segment failed",
        "We were unable to save your new data segment. Please try again later.": "We were unable to save your new data segment. Please try again later.",
        "Switch Segment Failed": "Switch Segment Failed",
        "We were unable to switch segments. Please try again later.": "We were unable to switch segments. Please try again later.",
        "You have already created a segment for that benchmark.": "You have already created a segment for that benchmark.",
        "Please change your segment choices and try again.": "Please change your segment choices and try again.",
        "EnableBenchmarks failed": "EnableBenchmarks failed",
        "We were unable to enable all your benchmarks at this time. Please try again later.": "We were unable to enable all your benchmarks at this time. Please try again later.",
        "Failed to Delete Segment": "Failed to Delete Segment",
        "We were unable to delete that data segment. Please try again later.": "We were unable to delete that data segment. Please try again later.",
        "Failed to save profile": "Failed to save profile",
        "We were unable to save your profile. Please try again later.": "We were unable to save your profile. Please try again later.",
        "Failed to Rename Segment": "Failed to Rename Segment",
        "We were unable to rename that data segment. Please try again later.": "We were unable to rename that data segment. Please try again later.",
        "Show/Hide Benchmark(s) failed": "Show/Hide Benchmark(s) failed",
        "We were unable to show or hide your benchmark(s) at this time. Please try again later.": "We were unable to show or hide your benchmark(s) at this time. Please try again later.",
        "I agree to anonymously contribute my Question Bank responses and profile information to Benchmarks.": "I agree to anonymously contribute my Question Bank responses and profile information to Benchmarks.",
        "Professional Services": "Professional Services",
        "Consumer Products": "Consumer Products",
        "Text Random Assignment - Text": "Text Random Assignment - Text",
        "Image Random Assignment - Image": "Image Random Assignment - Image",
        "Most Important": "Most Important",
        "Most Frequent": "Most Frequent",
        "A/B Test": "A/B Test"

    });
    /*</sl:translate_json>*/

    // -------------------------------------- Rules Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Filter by Question and Answer": "Filter by Question and Answer",
        "Filter by Collector": "Filter by Collector",
        "Filter by Completeness": "Filter by Completeness",
        "Filter by Time Period": "Filter by Time Period",
        "Filter by Respondent Metadata": "Filter by Respondent Metadata",
        "Filter by A/B Test": "Filter by A/B Test",
        "Compare by Question and Answer": "Compare by Question and Answer",
        "Compare by A/B Test": "Compare by A/B Test",
        "A/B TEST": "A/B TEST",
        "Choose a row...": "Choose a row...",
        "Choose a column...": "Choose a column...",
        "respondent metadata": "respondent metadata",
        "collector": "collector",
        "survey": "survey",
        "completeness": "completeness",
        "time period": "time period",
        "Complete responses": "Complete responses",
        "Partial responses": "Partial responses",
        "Disqualified responses": "Disqualified responses",
        "Responses over quota": "Responses over quota",
        "No response": "No response",
        "IP Address": "IP Address",
        "From Survey": "From Survey",
        "Email Address": "Email Address",
        "First Name": "First Name",
        "Last Name": "Last Name",
        "Custom Data": "Custom Data",
        "Please enter a valid IP address": "Please enter a valid IP address",
        "Please enter a valid email": "Please enter a valid email",
        "Respondent metadata filter": "Respondent metadata filter",
        "You can apply only one SHOW rule": "You can apply only one SHOW rule",
        "Show only certain questions": "Show only certain questions",
        "Compare is not allowed for Individual Responses": "Compare is not allowed for Individual Responses",
        "Compare is not allowed in Data Trends": "Compare is not allowed in Data Trends",
        "Compare is not allowed": "Compare is not allowed",
        "Crosstabulate your data": "Crosstabulate your data",
        "Choose": "Choose",
        "All Organizations": "All Organizations",
        "(Question Test)": "(Question Test)",
        "(Image Test)": "(Image Test)",
        "(Text Test)": "(Text Test)"
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Quotas Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "COMPLETE": "COMPLETE",
        "INCOMPLETE": "INCOMPLETE",
        "DISQUALIFIED": "DISQUALIFIED",
        "OVER QUOTA": "OVER QUOTA"
    });
    /*</sl:translate_json>*/

    // -------------------------------------- profiler Translations
    // here because the way profiler is doing it isn't working
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "_Profiler_Choose": "Choose",
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Exports Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Exports": "Exports",
        "Exporting your file...": "Exporting your file...",
        "Export complete": "Export complete",
        "Export failed": "Export failed",
        "Your export file is too large to process": "Your export file is too large to process",
        "There was a problem exporting your data": "There was a problem exporting your data",
        "Your export is complete": "Your export is complete",
        "Export files will appear under EXPORTS for 14 days.": "Export files will appear under EXPORTS for 14 days.",
        "A link to Google Drive will appear under EXPORTS for 14 days.": "A link to Google Drive will appear under EXPORTS for 14 days.",
        'Click "Download" to save the file to your computer.': 'Click "Download" to save the file to your computer.',
        "Opens in most analytics software": "Opens in most analytics software",
        "Opens in Microsoft Excel": "Opens in Microsoft Excel",
        "Open in advanced statistical and analytical software": "Open in advanced statistical and analytical software",
        "Provides a separate file for each database table": "Provides a separate file for each database table",
        "Best for adding charts as images to presentations": "Best for adding charts as images to presentations",
        "Ideal for sharing and opening on all computers": "Ideal for sharing and opening on all computers",
        "Ideal for presenting in Microsoft PowerPoint": "Ideal for presenting in Microsoft PowerPoint",
        "Open in your SPSS analytical software": "Open in your SPSS analytical software",
        "Ideal for posting directly to a website": "Ideal for posting directly to a website",
        "Ideal for sharing and printing": "Ideal for sharing and printing",
        "Ideal for presentations": "Ideal for presentations",
        "Please enter a valid filename": "Please enter a valid filename",
        "Max filename length is 250 characters": "Max filename length is 250 characters",
        "Downloads directly to Google Sheets": "Downloads directly to Google Sheets",
        "DRIVE":"DRIVE",
        "Complete Responses" : "Complete Responses",
        "Date Created": "Date Created",
        "Total Responses": "Total Responses",
        "Include open-ended responses": "Include open-ended responses",
        "Hide SurveyMonkey Branding": "Hide SurveyMonkey Branding",
        "Start each question on a new page": "Start each question on a new page",
        "Start each response on a new page": "Start each response on a new page",
        "Landscape (Horizontal)": "Landscape (Horizontal)",
        "Portrait (Vertical)": "Portrait (Vertical)",
        'Legal (8.5" x 14")': 'Legal (8.5" x 14")',
        'Letter (8.5" x 11")': 'Letter (8.5" x 11")',
        "A4 (210mm × 297mm)": "A4 (210mm × 297mm)",
        "Condensed": "Condensed",
        "Expanded":"Expanded",
        "Actual Answer Text": "Actual Answer Text",
        "Numerical Value (1-n)": "Numerical Value (1-n)"

    });
    /*</sl:translate_json>*/
    // -------------------------------------- Trends Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Zoom: ": "Zoom: ",
        " to ": " to ",
        "Weekly (Starting on the date)": "Weekly (Starting on the date)",
        "Quarterly (Starting on the date)": "Quarterly (Starting on the date)",
        "(by hour)": "(by hour)",
        "(by day)": "(by day)",
        "(by week)": "(by week)",
        "(by month)": "(by month)",
        "(by quarter)": "(by quarter)",
        "(by year)": "(by year)",
        "Responses (by hour)": "Responses (by hour)",
        "Responses (by day)": "Responses (by day)",
        "Responses (by week)": "Responses (by week)",
        "Responses (by month)": "Responses (by month)",
        "Responses (by quarter)": "Responses (by quarter)",
        "Responses (by year)": "Responses (by year)",
        "Data Trends do not apply to this question": "Data Trends do not apply to this question",
        "We are sorry.  There is too much data in your survey to display trends with that much detail.  Please select a longer time period in the Trend By menu to see your chart.": "We are sorry.  There is too much data in your survey to display trends with that much detail.  Please select a longer time period in the Trend By menu to see your chart."
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Sharing Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Shared Data": "Shared Data",
        "Enterprise Group": "Enterprise Group",
        "Password Restricted": "Password Restricted",
        "Public": "Public",
        "Anyone with the Link": "Anyone with the Link",
        "You copied your sharing web link.": "You copied your sharing web link.",
        "You can now paste the url into an email or social web site.": "You can now paste the url into an email or social web site.",
        "You must enter a title": "You must enter a title",
        "You must enter a nickname": "You must enter a nickname",
        "You must enter a description": "You must enter a description",
        "Please enter a description less than 4000 characters": "Please enter a description less than 4000 characters",
        "You must enter a password": "You must enter a password",
        "Please enter a password between 4 and 35 characters": "Please enter a password between 4 and 35 characters",
        "Turn sharing on": "Turn sharing on",
        "Turn sharing off": "Turn sharing off",
        "Click to view shared data":"Click to view shared data",
        " - Responses | SurveyMonkey": " - Responses | SurveyMonkey",
        "Not Available": "Not Available"
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Chart Customization Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Add": "Add",
        "Save": "Save",
        "Edit Color": "Edit Color",
        "Copy Color": "Copy Color",
        "Delete Color": "Delete Color",
        "Show and recalculate all": "Show and recalculate all",
        "Enter a number less than the lowest number in your chart": "Enter a number less than the lowest number in your chart",
        "Enter a number greater than the highest number in your chart": "Enter a number greater than the highest number in your chart"
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Survey Language Option Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Albanian": "Albanian",
        "Arabic": "Arabic",
        "Armenian": "Armenian",
        "Basque": "Basque",
        "Bengali":"Bengali",
        "Bosnian": "Bosnian",
        "Bulgarian": "Bulgarian",
        "Catalan": "Catalan",
        "Chinese (Simplified)": "Chinese (Simplified)",
        "Chinese (Traditional)": "Chinese (Traditional)",
        "Croatian": "Croatian",
        "Czech": "Czech",
        "Danish": "Danish",
        "Dutch": "Dutch",
        "English": "English",
        "Estonian": "Estonian",
        "Filipino": "Filipino",
        "Finnish": "Finnish",
        "French": "French",
        "Georgian": "Georgian",
        "German": "German",
        "Greek": "Greek",
        "Hebrew": "Hebrew",
        "Hindi": "Hindi",
        "Hungarian": "Hungarian",
        "Icelandic": "Icelandic",
        "Indonesian": "Indonesian",
        "Irish": "Irish",
        "Italian": "Italian",
        "Japanese": "Japanese",
        "Kurdish": "Kurdish",
        "Latvian": "Latvian",
        "Lithuanian": "Lithuanian",
        "Macedonian": "Macedonian",
        "Malay": "Malay",
        "Malayalam": "Malayalam",
        "Norwegian": "Norwegian",
        "Persian": "Persian",
        "Polish": "Polish",
        "Portuguese (Brazilian)": "Portuguese (Brazilian)",
        "Portuguese (Iberian)": "Portuguese (Iberian)",
        "Punjabi": "Punjabi",
        "Romanian": "Romanian",
        "Russian": "Russian",
        "Serbian": "Serbian",
        "Slovak": "Slovak",
        "Slovanian": "Slovanian",
        "Spanish": "Spanish",
        "Swedish": "Swedish",
        "Tamil": "Tamil",
        "Telugu": "Telugu",
        "Thai": "Thai",
        "Turkish": "Turkish",
        "Ukranian": "Ukranian",
        "Vietnamese": "Vietnamese",
        "Welsh": "Welsh"
    });
    /*</sl:translate_json>*/

    // -------------------------------------- Survey Theme Translations
    /*<sl:translate_json>*/
    SM.Object.update(SM.translations, {
        "sl_translate": "sl_all",
        "Aqua": "Aqua",
        "Anemone": "Anemone",
        "Berries": "Berries",
        "Chestnut": "Chestnut",
        "Denim": "Denim",
        "Modern Monkey": "Modern Monkey",
        "Panda": "Panda",
        "Rain": "Rain",
        "Seriously Blue": "Seriously Blue",
        "Summer": "Summer",
        "Velvet": "Velvet",
        "Vintage": "Vintage"
    });
    /*</sl:translate_json>*/
    // -------------------------------------- Server Translations
    /*<sl:translate_json>*/
    serverTranslations = {
        "sl_translate": "sl_all",
        "Original View": "Original View",
        
        "sl_translate": "sl_all"
    };
    /*</sl:translate_json>*/

    for (translation in serverTranslations) {
        SM.translations[translation] = serverTranslations[translation];
    }

    // -------------------------------------- Apply

    culture = Globalize.getSmartlingCulture();
    Globalize.culture(culture);
    Globalize.addCultureInfo(culture, {
        messages: SM.translations
    });

})();
</script>

    <script type="text/javascript">
        SM.SurveySummaryApp.init({
            data_url: "//www.surveymonkey.com/summary/VXWbm7jkt_2FH0pjzX5h9xAfZrIeBBCJdDfvDDQBybwQU_3D/data.js?",
            el: $("[survey-summary-layout]").get(0),
            survey_id: "77461121",
            version: "88.5.247",
            notif_e_opt_out: "-1"
        });
    </script>


        
            
            
            <script type="text/javascript">
                var data_layer = {
                    
                    user_id: "88419848",
                    package_id: "",
                    country_code: "US",
                    language_id: "en",
                    
                    sip: "184",
                    current_datetime: "2016-06-04 23:24:03"
                }
            </script>
        

        
    </body>
</html>