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
<div id="tpName" itemprop="name" style="font-size: 11pt; color: #369; font-weight: bold;">Team Person</div>

<div id="tp_details" style="color: #99a;">M: <span itemprop="telephone" id="tpPhone">+44 71234 567890</span> |  <a id="tpEmail" itemprop="email" href="mailto:first.last@teampolice.uk">first.last@teampolice.uk</a></div>
<div id="tp_logo"><a href="https://www.teampolice.uk/"><img src="https://ethosvo.github.io/ethos-email-signature/teampolice-generic.png" style="width: 300px; height: 76px" alt="TeamPolice Logo"></a></div>
<div id="tp_strap"><a href="http://eepurl.com/gMRNSb">Sign up to our newsletter</a> and we’ll keep you informed on the latest news from TeamPolice</div>
<div id="tp_socialmedia">
<a href="https://www.facebook.com/TeamPoliceUK"><img src="https://ethosvo.github.io/ethos-email-signature/social/facebook.png" style="vertical-align: text-bottom; width: 16px; height: 16px" alt="Facebook"> Facebook</a>
<a href="https://twitter.com/teampoliceuk"><img src="https://ethosvo.github.io/ethos-email-signature/social/twitter.png" style="vertical-align: text-bottom;margin-left: 10px; width: 16px; height: 16px" alt="Twitter"> Twitter</a>
<a href="https://www.instagram.com/teampoliceuk/"><img src="https://ethosvo.github.io/ethos-email-signature/social/instagram.png" style="vertical-align: text-bottom;margin-left: 10px; width: 16px; height: 16px" alt="Instagram"> Instagram</a>
<a href="https://www.linkedin.com/company/teampolice/"><img src="https://ethosvo.github.io/ethos-email-signature/social/linkedin.png" style="vertical-align: text-bottom;margin-left: 10px; width: 16px; height: 16px" alt="LinkedIn"> LinkedIn</a>
<a href="https://www.teampolice.uk/"><img src="https://ethosvo.github.io/ethos-email-signature/social/website.png" style="vertical-align: text-bottom;margin-left: 10px; width: 16px; height: 16px" alt="Website"> www.teampolice.uk</a>
</div>
    </section>
    </div>
</div><!-- end of resBox -->

<h2>What Next?</h2>

<p>Use your mouse to select everything in the generated signature, from your Name to the social media icons. Copy this (Ctrl+C on a Windows PC).</p>

<p>Next, go to your <a target="_blank" href="https://mail.google.com/mail/#settings/general">signature settings in Gmail</a>. Find &quot;Signature&quot; section.</p>

<p>If you don't already have a signature, create one now.</p>

<p>Paste (Ctrl+V) the signature into the signature editor.</p>

<p>Scroll to the bottom of the page and click Save Changes.</p>

<p>Now, whenever you create an email, you will have the option (little pen icon) to add a TeamPolice signature.</p>




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
            tpEmail.setAttribute("href", "mailto:" + frm.email.value);
        }
        




    })();
</script>