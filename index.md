---
title: "Free Android GPS Logger for Photographers"
description: "Lightweight, and ad-free Android GPS logger designed specifically for photographers and seamless geotagging workflows."
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

/* Profesionální styl pro klikací screenshoty */
.screenshot-link {
  display: block;
  margin: 24px auto;
  max-width: 100%;
  text-decoration: none;
}
.screenshot-img {
  width: 100%;
  height: auto;
  display: block;
  border: 1px solid #333;
  border-radius: 8px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.18);
  transition: transform 0.2s ease, opacity 0.2s ease;
}
.screenshot-img:hover {
  opacity: 0.96;
  transform: translateY(-2px);
}

/* Badge a alert boxy */
.update-badge {
  display: inline-block;
  background-color: #2ea44f;
  color: #ffffff;
  font-size: 13px;
  font-weight: 600;
  padding: 4px 10px;
  border-radius: 20px;
  margin-bottom: 12px;
}

.notice-box {
  background: #f6f8fa;
  border: 1px solid #d0d7de;
  border-left: 4px solid #0969da;
  border-radius: 6px;
  padding: 14px 18px;
  margin: 20px 0;
  font-size: 14px;
}

@media (prefers-color-scheme: dark) {
  .notice-box {
    background: #161b22;
    border-color: #30363d;
    border-left-color: #58a6ff;
    color: #c9d1d9;
  }
}

/* GitHub Téma vyhledávacího komponentu (Světlý i Tmavý režim) */
#flex-search-container {
  max-width: 500px;
  margin: 25px auto;
  position: relative;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", Helvetica, Arial, sans-serif;
}

#flex-search-input {
  width: 100%;
  padding: 12px 16px;
  font-size: 14px;
  line-height: 20px;
  border-radius: 6px;
  box-sizing: border-box;
  transition: border-color 0.2s, box-shadow 0.2s, background-color 0.2s, color 0.2s;
  border: 1px solid #d0d7de;
  background-color: #f6f8fa;
  color: #24292f;
}

#flex-search-input::placeholder {
  color: #57606a;
  opacity: 1;
}

#flex-search-input:focus {
  outline: none;
  background-color: #ffffff;
  border-color: #0969da;
  box-shadow: 0 0 0 3px rgba(9, 105, 218, 0.3);
}

#flex-results-container {
  position: absolute;
  top: 100%;
  left: 0;
  width: 100%;
  border-radius: 6px;
  list-style: none;
  padding: 0;
  margin: 8px 0 0 0;
  z-index: 100;
  max-height: 300px;
  overflow-y: auto;
  display: none;
  background-color: #ffffff;
  border: 1px solid #d0d7de;
  box-shadow: 0 8px 24px rgba(140, 149, 159, 0.2);
}

#flex-results-container li {
  border-bottom: 1px solid #d0d7de;
}

#flex-results-container li:last-child {
  border-bottom: none;
}

#flex-results-container li a {
  display: block;
  padding: 12px 16px;
  text-decoration: none;
  font-size: 14px;
  font-weight: 500;
  color: #24292f;
  transition: background-color 0.1s, color 0.1s;
}

#flex-results-container li a:hover {
  background-color: #0969da;
  color: #ffffff;
}

#flex-results-container .no-results-msg {
  padding: 12px 16px;
  color: #57606a;
  font-style: italic;
  font-size: 14px;
}

@media (prefers-color-scheme: dark) {
  #flex-search-input {
    border: 1px solid #30363d;
    background-color: #0d1117;
    color: #c9d1d9;
  }
  #flex-search-input::placeholder {
    color: #8b949e;
  }
  #flex-search-input:focus {
    border-color: #58a6ff;
    box-shadow: 0 0 0 3px rgba(88, 166, 255, 0.3);
  }
  #flex-results-container {
    background-color: #161b22;
    border: 1px solid #30363d;
    box-shadow: 0 8px 24px rgba(1, 4, 9, 0.8);
  }
  #flex-results-container li {
    border-bottom: 1px solid #21262d;
  }
  #flex-results-container li a {
    color: #c9d1d9;
  }
  #flex-results-container li a:hover {
    background-color: #1f6feb;
    color: #ffffff;
  }
  #flex-results-container .no-results-msg {
    color: #8b949e;
  }
}
</style>
</div>

# Free Artush GPX Tracker

<div style="width: 100%; max-width: 1200px; margin: 0 auto 20px auto; background: transparent; line-height: 0;">
  <object type="image/svg+xml" data="artushGPXtracker.svg" title="Artush GPX Tracker" style="width: 100%; height: auto; aspect-ratio: 841.89 / 200; display: block; border: none; margin: 0; padding: 0; pointer-events: auto !important;">
    <img src="artushGPXtracker.svg" alt="Artush GPX Tracker" style="width: 100%; height: auto; display: block;" />
  </object>
</div>

**Lightweight, single-purpose, and ad-free Android GPS logger designed for photographers.**

**Artush GPX Tracker** provides straightforward, precise GPS track recording in **UTC** time. It is crafted as the ideal mobile companion for matching geographic coordinates to photos in [**ArtushVision AI - Professional Metadata Automation**](https://vision.artushfoto.eu), as well as in any other photo editor that supports GPX geotagging.

---

## How Does Photo Geotagging Work?

**Add GPS location to your photos even if your camera doesn't have built-in GPS!**
You don't need a special camera, GPS accessories, or complicated cables. All you need is your smartphone and a simple GPS tracking app.

### 1. Your Phone Records Where You Go
Start **Artush GPX Tracker** on your phone before you begin taking pictures. Keep it in your pocket or camera bag.
The app automatically records your location and the exact time as you move around. It saves everything in a standard `.gpx` track file.

### 2. Your Camera Records When You Take Photos
Every time you press the shutter, your camera saves the date and time of the shot inside the photo.
This works with virtually any digital camera, including older DSLR models without GPS.

### 3. Your Photos Get Their GPS Location
After your photoshoot, simply load your photos and GPX track into [ArtushVision AI - Professional Metadata Automation](https://vision.artushfoto.eu), Lightroom Classic, digiKam, or other compatible software.
The software matches the time of each photo with your recorded GPS track and automatically finds where you took the picture.
It then adds the GPS coordinates to your photo's metadata.

**That's it!** Your photos now contain their geographical location, ready for sorting, mapping, and uploading to stock photography agencies.

---

### Why Should You Synchronize Your Camera Clock?

Your camera and phone need to agree on the time to correctly match photos with GPS locations.

Over time, your camera's internal clock may become a few seconds or even minutes inaccurate.

Artush GPX Tracker includes a simple solution:

1. Open the Clock screen in the app.
2. Take a photograph of your phone's displayed clock using your camera.
3. Load this reference photo into ArtushVision AI.
4. The software automatically calculates the time difference and corrects the synchronization.

**No manual calculations. No guessing. Even older cameras can produce accurately geotagged photos.**

---

### Perfect for Every Photography Adventure

Whether you photograph wildlife, landscapes, nature or travel, Artush GPX Tracker quietly records your journey in the background.

* **Wildlife Photography:** Record the exact locations where you photograph animals, even during long waits in one place.
* **Landscape Photography:** Remember the exact viewpoints and locations of your favorite compositions.
* **Travel Photography:** Keep a GPS record of your entire photographic journey.
* **Nature Photography:** Easily find the locations of plants, flowers and other natural subjects.

Your phone records the locations. Your camera captures the moments. Your photos remember both.

---

<p align="center">
  <img src="images/start-recording.webp" width="22%" alt="App screen before starting track recording">
  <img src="images/recording.webp" width="22%" alt="App screen during active track recording">
  <img src="images/tracks.webp" width="22%" alt="App screen showing list of saved tracks">
  <img src="images/clock.webp" width="22%" alt="App screen showing camera clock synchronization">
</p>

## Key Features and Benefits
Everything you need to remember where you took your photos – simple, reliable and ready for your next photography adventure.

* **Accurate GPS Recording**
Record your geographic locations with precise timestamps, making it easy to match your photos with the correct GPS coordinates.

* **Continuous Location Tracking**
Your phone records your location even when you stop moving to photograph wildlife, landscapes or other subjects.

* **Safe Track Storage**
Your recorded GPS tracks are saved and remain available when you close the app or restart your phone.

* **Simple and Easy to Use**
A clean, intuitive interface makes GPS tracking easy on different Android phone screens.

* **Track History & Management**
View, browse, rename and manage your previously recorded photography trips.

* **Interactive Map**
See your recorded routes and discover exactly where you took your photographs.

* **Camera Clock Synchronization**
Easily check and correct your camera's clock to ensure your photos receive the right GPS locations.

* **Standard GPX Export**
Export your GPS tracks in the widely supported GPX format and use them with [**ArtushVision AI - Professional Metadata Automation**](https://vision.artushfoto.eu), Lightroom-compatible workflows and other geotagging software.

* **Customizable Settings & Multilingual Support:** 
Easily toggle between languages (Czech, English, German, Spanish, French, Italian, Polish, Slovak, Portuguese, Russian, Hungarian, Ukrainian, Vietnamese, Korean, Chinese, Japanese, Arabic, Hebrew, Turkish) and adjust logging intervals (1s to 1min).

---

## App Controls & Navigation

The app is organized into 4 clear tabs in the bottom navigation bar:

### 1. Record
* **Tracking HUD:**
  * **Service:** Indicates live tracking status (`SERVICE ACTIVE` / `SERVICE STOPPED`).
  * **Start & Duration:** Displays start time in UTC and a live elapsed timer.
  * **Fix Quality:** Instant visual indicator of GPS accuracy (🟢 High Accuracy, 🟠 Usable, 🔴 No Signal).
  * **Telemetry:** Displays the age of the latest point, accuracy in meters, altitude, and total recorded points.
* **Action Buttons:**
  * **[Show on Map]:** Opens Google Maps centered on your current location.
  * **[▶ START LOGGING / ■ STOP LOGGING]:** Starts or stops background track recording. When starting, the app prompts you to either continue the existing track or begin a new one.
  * **[Map]:** Opens the complete GPX track in Mapy.cz or Google Earth.
  * **[Share]:** Instantly sends the GPX file to your PC or cloud storage (Quick Share, Email, Google Drive).

### 2. Tracks
* Complete history of all stored tracks.
* Each entry shows title, date, start/end timestamps, and recorded point count.
* **Track Actions:**
  * ✏ **Rename Track** (e.g., *Iguazu Falls - Autumn Shoot*).
  * 📝 **Add Note / Description**. (Exported alongside GPX as a .txt file with the same name)
  * 🗺️ **Open in Map App**.
  * 📤 **Share GPX**.
  * 🗑️ **Delete Track**.

### 3. Clock
* Pure black AMOLED background with large local and UTC time displays, including milliseconds.
* Photograph this screen with your camera before or during your shoot. Then, enter the visible time into the [**ArtushVision AI - Professional Metadata Automation**](https://vision.artushfoto.eu) time-shift calculator to synchronize photos with your GPX track automatically.

<p align="center">
  <img src="images/rename-note.webp" width="22%" alt="Artush GPX Tracker Rename track or write note">
  <img src="images/settings1.webp" width="22%" alt="Artush GPX Tracker Select language">
  <img src="images/settings2.webp" width="22%" alt=" Artush GPX Tracker Set update interval">
  <img src="images/settings3.webp" width="22%" alt="Artush GPX Tracker Quick guide">
</p>

---

## Photo Geotagging & Synchronization

Exported `.gpx` files strictly follow the **GPX 1.1** standard, ensuring compatibility with all major geotagging software:

### 1. ArtushVision AI (Recommended) 💻
[**ArtushVision AI – Professional Metadata Automation**](https://vision.artushfoto.eu) is an advanced Windows desktop tool for automated captioning, keyword management, and rapid GPS track synchronization:
* **Effortless Time Offset Calculation**: Simply load the reference photo of the Artush GPX Tracker's **Clock Sync** screen and enter the time displayed on it. ArtushVision AI instantly compares that time against the photo's capture timestamp and calculates the exact time difference automatically.
* **Precise Geotagging**: The application writes the synchronized GPS coordinates directly into your photos' EXIF/XMP metadata.

<a href="images/time-sync-in-artushvision-ai.webp" target="_blank" class="screenshot-link">
  <img src="images/time-sync-in-artushvision-ai.webp" alt="ArtushVision AI window for easy clock synchronization between camera and GPS data" width="100%" class="screenshot-img">
</a>
<div style="height: 5px;"></div>

### 2. Adobe Lightroom Classic
* In the **Map** module, select *Tracklog ➔ Load Tracklog...* and pick the file exported from Artush GPX Tracker.
* Lightroom automatically positions photos on the map using matching EXIF timestamps.

### 3. Zoner Photo Studio X
* In the **Manager** module, select your photos and go to *Map ➔ Assign GPS from GPX File...*.

### 4. Other Compatible Software
* **GeoSetter**, **Darktable**, **DigiKam**, **Apple Photos**, and any other software supporting GPX 1.1.

---

## Installation

1. **Download the APK:** Scan the QR code below using your mobile device or click the link to download the installation package directly to your Android phone. *(Note: Official Google Play release is currently in progress).*
2. **Installation Guide**: When installing the APK manually outside Google Play, Android will prompt you to grant permission to **"Install unknown apps"** for your web browser or file manager.
3. **Complete Installation:** Open the downloaded file, confirm the installation, and you are ready to start tracking your GPS routes.

---

## Links & Downloads

* **Artush GPX Tracker (🤖 Android Mobile App)** Will be available soon (Google Play approval is in process)

[**Click here to become a beta tester for Artush GPX Tracker, or scan the QR code with your phone.**](https://play.google.com/apps/testing/com.artush.gpxtracker)
    
<p align="left">
  <img src="become-tester.png" width="15%" alt="Test Artush GPX Tracker">
</p>

---

[**ArtushVision AI - Professional Metadata Automation (Desktop Software)**](https://vision.artushfoto.eu)
* The Ultimate AI-Powered Workstation for Metadata, Asset Management, and Global & FTP Distribution.
---

### Privacy, Permissions & Security

* **Location Permission Only**: The application requires only **location access** (*Foreground* and *Background Location*) exclusively to record your route coordinates into GPX tracks. It does not request access to your private files, contacts, camera, or microphone.

[📷 Developer's Photography Portfolio: artushfoto.eu](https://artushfoto.eu)

---

*ArtushVision AI — intelligent metadata optimization for professional photography workflows.*

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