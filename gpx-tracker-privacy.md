---
title: "Privacy Policy - Artush GPX Tracker"
description: "Privacy Policy and data handling practices for the Artush GPX Tracker Android application."
---

<!-- Cookie Consent Styly a Skript -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/cookieconsent@3/build/cookieconsent.min.css" />
<script src="https://cdn.jsdelivr.net/npm/cookieconsent@3/build/cookieconsent.min.js"></script>
<script>
window.addEventListener("load", function() {
  window.cookieconsent.initialise({
    "palette": {
      "popup": { "background": "#24292f", "text": "#ffffff" },
      "button": { "background": "#2ea44f", "text": "#ffffff" }
    },
    "theme": "classic",
    "position": "bottom",
    "type": "opt-in",
    "content": {
      "message": "This website uses cookies to ensure you get the best experience and to measure traffic.",
      "dismiss": "Decline",
      "allow": "Allow cookies",
      "link": "Learn more"
    },
    onStatusChange: function(status) {
      if (this.hasConsented()) {
        if (typeof window.loadAnalyticsAfterConsent === 'function') {
          window.loadAnalyticsAfterConsent();
        }
      }
    }
  });
});
</script>

<div style="display: none;">
<style>
header, .page-header, .site-header, footer, .site-footer, .footer, .page-title, .project-name, a.project-banner, section.page-header { display: none !important; }
h1 { text-align: center; }
.privacy-container {
  max-width: 800px;
  margin: 40px auto;
  padding: 0 20px;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", Helvetica, Arial, sans-serif;
  line-height: 1.6;
  color: #24292f;
}
@media (prefers-color-scheme: dark) {
  .privacy-container { color: #c9d1d9; }
}
</style>
</div>

<div class="privacy-container" markdown="1">

# Privacy Policy for Artush GPX Tracker

**Effective date:** October 6, 2026

Artush ("we", "our", or "us") built the **Artush GPX Tracker** app as a free utility app. This SERVICE is provided by us at no cost and is intended for use as is.

This page is used to inform visitors regarding our policies with the collection, use, and disclosure of Personal Information if anyone decided to use our Service.

### Information Collection and Use
To provide the core functionality of tracking and recording your outdoor routes (GPX tracks), the app requires access to your device's location data. 
* **Location Data:** The app collects and processes your GPS location data in real-time strictly while you are actively recording a track or using the tracking features. 
* **Data Storage:** All recorded GPX tracks and location data are stored locally on your device. We do not transmit, sell, or share your location data or personal information to any external servers or third parties.

### Third-Party Services
The app does not use any third-party tracking, analytics, or advertising SDKs that collect personal or location data. 

### Security
We value your trust in providing us your location data, thus we are striving to use commercially acceptable means of protecting it. But remember that no method of transmission over the internet, or method of electronic storage is 100% secure and reliable, and we cannot guarantee its absolute security.

### Children’s Privacy
Our Services do not address anyone under the age of 13. We do not knowingly collect personally identifiable information from children under 13. 

### Changes to This Privacy Policy
Our Privacy Policy may be updated from time to time. Thus, you are advised to review this page periodically for any changes. We will notify you of any changes by posting the new Privacy Policy on this page.

### Contact Us
If you have any questions or suggestions about our Privacy Policy, do not hesitate to contact us at:
* **Email:** artushfoto@gmail.com

---

[📷 Developer's Photography Portfolio: artushfoto.eu](https://artushfoto.eu)

</div>

<!-- Odložené a podmíněné načtení Google Analytics s ohledem na Cookie Consent -->
<script>
  window.loadAnalyticsAfterConsent = function() {
    if (window.analyticsLoaded) return;
    window.analyticsLoaded = true;

    var gtagScript = document.createElement('script');
    gtagScript.async = true;
    gtagScript.src = 'https://www.googletagmanager.com/gtag/js?id=G-H4FSFZTMXH';
    document.head.appendChild(gtagScript);

    window.dataLayer = window.dataLayer || [];
    window.gtag = function(){ dataLayer.push(arguments); }
    gtag('js', new Date());
    gtag('config', 'G-H4FSFZTMXH');
  };

  document.addEventListener("DOMContentLoaded", function() {
    function checkConsentAndLoad() {
      const cookieConstData = document.cookie;
      if (cookieConstData.indexOf('cookieconsent_status=allow') !== -1) {
        window.loadAnalyticsAfterConsent();
        return;
      }
      
      let analyticsLoaded = false;
      function triggerOnInteraction() {
        if (analyticsLoaded) return;
        if (document.cookie.indexOf('cookieconsent_status=allow') !== -1) {
          analyticsLoaded = true;
          window.loadAnalyticsAfterConsent();
          document.removeEventListener('scroll', triggerOnInteraction);
          document.removeEventListener('mousemove', triggerOnInteraction);
        }
      }
      document.addEventListener('scroll', triggerOnInteraction, { passive: true });
      document.addEventListener('mousemove', triggerOnInteraction, { passive: true });
    }

    setTimeout(checkConsentAndLoad, 1000);
  });
</script>