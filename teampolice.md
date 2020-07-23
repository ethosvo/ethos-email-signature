---
layout: default
title: TeamPolice
---

<style>
form { margin: 20px; }
#resBox { margin: 40px 0; }
label { width: 100%; }
label input { float: right; width: 50%; }


</style>

<h1>TeamPolice Email Signature</h1>

<p>Use the following form to generate your TeamPolice signature:</p>

<form name="userdetails">
    <div><label>Your Name<input autofocus type="text" name="name"></label></div>
    <div><label>Your Phone Number<input type="text" name="phone"></label></div>
    <div><label>Your Email Address<input type="email" name="email"></label></div>
</form>

<div id="resBox">

<div id="resPreview">
<section id="tp_emailblock" itemscope itemtype="http://schema.org/Person" style="font: 9pt sans-serif; line-height: 22pt; ">
<div id="tpName" itemprop="name" style="font-size: 11pt; color: #369; font-weight: bold;">Annabelle Lambert</div>

<div id="tp_details" style="color: #99a;">M: <span id="tpPhone">+44 [0]794 1253867</span> |  <a id="tpEmail" href="mailto:annabelle.lambert@teampolice.uk">annabelle.lambert@teampolice.uk</a></div>
<div id="tp_logo"><img src="https://ethosvo.github.io/ethos-email-signature/teampolice-generic.png" style="width: 150px; height: 38px" alt="TeamPolice Logo"></div>
<div id="tp_strap"><a href="http://eepurl.com/gMRNSb">Sign up to our newsletter</a> and we’ll keep you informed on the latest news from TeamPolice</div>
<div id="tp_socialmedia">
<a href="https://www.facebook.com/TeamPoliceUK"><img src="https://ethosvo.github.io/ethos-email-signature/social/facebook.png" style="width: 58px; height: 58px" alt="Facebook"></a>
<a href="https://twitter.com/teampoliceuk"><img src="https://ethosvo.github.io/ethos-email-signature/social/twitter.png" style="width: 50px; height: 50px" alt="Twitter"></a>
<a href="https://www.instagram.com/teampoliceuk/"><img src="https://ethosvo.github.io/ethos-email-signature/social/instagram.png" style="width: 50px; height: 50px" alt="Instagram"></a>
</div>
    </section>
    </div>
</div><!-- end of resBox -->

<script>
    (function() {
        var frm = document.forms.userdetails;
        var resBox = document.getElementById("resBox");

        frm.addEventListener("submit", function(ev) { ev.preventDefault(); });
        frm.name.addEventListener("change", function() { updatePreview(); });
        frm.name.addEventListener("keyup", function() { updatePreview(); });
        frm.email.addEventListener("change", function() { updatePreview(); });
        frm.email.addEventListener("keyup", function() { updatePreview(); });
        frm.phone.addEventListener("change", function() { updatePreview(); });
        frm.phone.addEventListener("keyup", function() { updatePreview(); });

// Template objects:
var tpName = document.getElementById("tpName");
var tpPhone = document.getElementById("tpPhone");
var tpEmail = document.getElementById("tpEmail");
var resPreview = document.getElementById("resPreview");
        function updatePreview() {
            tpName.innerHTML = tpPhone.innerHTML = tpEmail.innerHTML = '';
            tpName.appendChild(document.createTextNode(frm.name.value));
            tpPhone.appendChild(document.createTextNode(frm.phone.value));
            tpEmail.appendChild(document.createTextNode(frm.email.value));
        }
        




    })();
</script>