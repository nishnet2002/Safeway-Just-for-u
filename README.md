SafewayJ4U-Bookmarklet
======================

SafewayJ4U

1. Copy the text in bookmarklet.txt - javascript:(function(e,a,g,h,f,c,b,d){if(!(f=e.jQuery)||g>f.fn.jquery||h(f)){c=a.createElement("script");c.type="text/javascript";c.src="http://ajax.googleapis.com/ajax/libs/jquery/"+g+"/jquery.min.js";c.onload=c.onreadystatechange=function(){if(!b&&(!(d=this.readyState)||d=="loaded"||d=="complete")){h((f=e.jQuery).noConflict(1),b=1);f(c).remove()}};a.documentElement.childNodes[0].appendChild(c)}})(window,document,"1.7.2",function($,L){function processOffers(e){var t=e.offers;for(var n=0;n<t.length;n++){var r=t[n];if(r.clipStatus==="U"){var i=[];var s={};s.offerId=r.offerId;s.offerPgm=r.offerPgm;i.push(s);var o={};o.clips=i;var u=JSON.stringify(o);$.ajax({type:"POST",url:"http://www.safeway.com/Clipping1/services/clip/offers",contentType:"application/json",data:u})}}}$(document).ready(function(){var e=[];console.log("Making Request CC");$.ajax("http://www.safeway.com/J4UProgram1/services/program/CC/offer/allocations").done(processOffers);$.ajax("http://www.safeway.com/J4UProgram1/services/program/PD/offer/allocations").done(processOffers)})});
2. Create a bookmark in your favourite browser.
3. Visit Safeway and signin (makesure you visit the FULL site and not mobile site.)
4. Click the bookmark you just created.
