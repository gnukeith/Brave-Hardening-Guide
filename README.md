<h1 align= "center">Brave-Hardening-Guide<h1>

<p align="center">How to make Brave browser as private as possible</p>

<h2 align="center">What is the Brave browser?</h2>

<p align="center">The Brave browser is a free, open-source  web browser that prioritizes user privacy and security. It's built on the Chromium web browser, which is the foundation for Google Chrome. Brave is known for its built-in ad-blocking and tracking protection, which can make browsing faster and more private. It also offers a unique feature called Brave Rewards, where users can earn cryptocurrency (Basic Attention Token or BAT) for viewing privacy-respecting ads. Additionally, Brave has a built-in cryptocurrency wallet called Brave Wallet and a firewall and VPN service called Brave Firewall + VPN, which are available as paid options.</p>

*Brave source code can be found here:* https://github.com/brave/brave-core

<p align="center">Brave is also known for its speed and efficiency. It's designed to use less memory and battery life compared to other browsers, which can be beneficial for users on mobile devices or older computers.</p>

<p align="center">Overall, the Brave browser is a good choice for users who value privacy and security, and who want a browser that's fast and efficient.</p>

<h2 align="center">Why Harden Brave?</h2>
<p align="center">Even though Brave is designed to protect your privacy, there are additional steps you can take to enhance its security and privacy features further. Here's why you might want to harden Brave:</p>

<h3 align="center">Eliminate Telemetry</h3>
<p align="center">By default, Brave sends anonymous telemetry data. Hardening Brave can disable this data collection, ensuring that no information about your browsing habits is sent back to Brave's servers.</p>

<h3 align="center">Block More Ads and Trackers</h3>
<p align="center">Hardening Brave makes the browser more aggressive at blocking ads and trackers. This means you are less likely to encounter unwanted ads, making your browsing experience faster and more private.</p>
<p align="center">In summary, hardening Brave can make it an even more private and secure browser by stopping all telemetry and enhancing ad and tracker blocking capabilities.</p>

<h2 align="center">How to Harden Brave</h2>
<p align="center">Here are some steps you can take to harden Brave and make it as private as possible:

</p>
<h3 align="center">1. Hardening via Brave Sheild</h3>
<p align="center">Brave Shield is a built-in feature that allows you to control the browser's ad-blocking and tracking protection settings. You can access Brave Shield by clicking on the lion icon in the address bar or going to: brave://settings/shields. Here are some settings you can adjust to enhance your privacy:</p>

<h3 align="center">By default the settings should look something like this:</h3>

<p align="center">
    <img src="img/brave_shield_before.png" alt="Brave Shield Before">
</p>

<h3 align="center">After hardening the settings should look like this:</h3>

<p align="center">
    <img src="img/brave_shield_after.png" alt="Brave Shield After">
</p>

<p align="center">


## Before Hardening (Default Settings)

1. **Show the number of blocked items on the Shields icon:**
   - **On:** Displays a count of the blocked items (trackers, ads, etc.) directly on the Shields icon, giving you a quick overview of what's being blocked on the current page.

2. **Trackers & ads blocking:**
   - **Standard:** Blocks a balanced amount of trackers and ads to enhance privacy without breaking many websites.

3. **Upgrade connections to HTTPS:**
   - **Standard:** Automatically upgrades your connections to HTTPS where possible, ensuring that your data is encrypted.

4. **Block scripts:**
   - **Off:** Allows all scripts to run on websites. Scripts can enhance functionality but may also be used for tracking or malicious purposes.

5. **Block fingerprinting:**
   - **On:** Prevents websites from uniquely identifying your browser and device configuration, enhancing your privacy.

6. **Block cookies:**
   - **Block third-party cookies:** Prevents cookies from external sites (not the one you're visiting) from being stored, reducing tracking by advertisers.

7. **Forget me when I close this site:**
   - **On:** Deletes cookies and site data when you close the site, ensuring no data is stored between sessions.

8. **Content filtering:**
   - **Disabled:** No custom filters are applied to block additional regional or language-specific trackers and annoyances.

## After Hardening

1. **Show the number of blocked items on the Shields icon:**
   - **On:** Same as before, it shows the count of blocked items on the Shields icon.

2. **Trackers & ads blocking:**
   - **Aggressive:** Blocks a larger number of trackers and ads, increasing privacy but potentially causing more websites to break or function improperly.

3. **Upgrade connections to HTTPS:**
   - **Strict:** Forces all connections to HTTPS, providing maximum encryption but possibly causing issues with websites that do not support HTTPS.

4. **Block scripts:**
   - **Off:** Same as before, allows all scripts to run.

5. **Block fingerprinting:**
   - **On:** Same as before, continues to block fingerprinting techniques.

6. **Block cookies:**
   - **Block third-party cookies:** Same as before, blocking third-party cookies.

7. **Forget me when I close this site:**
   - **On:** Same as before, deletes cookies and site data when you close the site.

   **Note:** This setting can log you out of websites each time you close them, so be aware of this behavior.

   You can whitelist sites where you want to stay logged in by clicking on the Brave Shields icon and adjusting the settings for that specific site.

    <img src="img/cookies_whitelist.png" alt="Whitelisting">

8. **Content filtering:**
   - **Disabled:** Same as before, no custom filters are applied.

## Summary

By hardening Brave, you mainly enhance its ability to block ads and trackers more aggressively and ensure stricter HTTPS connections. These changes improve privacy and security but may affect website functionality.

## Important Note on Script and Cookie Blocking

### Script Blocking

While Brave offers the option to block scripts, it's important to note that enabling this feature will likely break many websites and is not recommended for daily use unless absolutely necessary. Most modern websites rely heavily on JavaScript for their functionality, and blocking scripts can severely impact your browsing experience.

If you do choose to block scripts:
- Many interactive features on websites will not work
- Some websites may fail to load entirely
- You may need to frequently toggle this setting on and off to use certain sites

The "Block" button for scripts in Brave's settings, when enabled, prevents JavaScript from running on the websites you visit. This can enhance privacy and security by preventing potentially malicious scripts from executing, but it comes at the cost of reduced functionality on most websites.

For most users, it's recommended to keep script blocking turned off and rely on Brave's other privacy features, which provide a good balance between security and usability.

### Cookie Blocking

Brave allows you to choose between blocking all cookies or just third-party cookies. Here's what you need to know:

#### Blocking All Cookies:
- **Pros:** Maximum privacy as websites can't store any information about your visits.
- **Cons:** 
  - You'll be logged out of all websites each time you close your browser.
  - Many websites will not function properly or remember your preferences.
  - You may need to enter login information frequently.
  - Some online services, like shopping carts, may not work correctly.

#### Blocking Only Third-Party Cookies (Recommended):
- **Pros:** 
  - Blocks tracking cookies from external sites, enhancing privacy.
  - Allows first-party cookies, maintaining functionality for most websites.
- **Cons:** 
  - Some cross-site features might not work properly.
  - Some tracking is still possible through first-party cookies.

It's generally recommended to block only third-party cookies as this provides a good balance between privacy and usability. This setting allows websites to remember your login status and preferences while still blocking many tracking attempts from external sources.

For most users, blocking third-party cookies combined with Brave's other privacy features offers a solid level of protection without significantly impacting your browsing experience.
</p>

<p align="center">

## Social Media Blocking

### Before Hardening (Default Settings)

1. **Allow Facebook logins and embedded posts:**
   - **On:** Enables Facebook logins and embedded Facebook content (such as posts and comments) on websites.

2. **Allow X (previously Twitter) embedded tweets:**
   - **On:** Allows embedded tweets from X (Twitter) to appear on websites.

3. **Allow LinkedIn embedded posts:**
   - **Off:** Blocks embedded LinkedIn content, preventing LinkedIn from tracking your activity through these embeds.


<img src="img/smb_before.png" alt="Brave Shield Before">


### After Hardening

1. **Allow Facebook logins and embedded posts:**
   - **Off:** Blocks Facebook logins and embedded content, preventing Facebook from tracking your activity on other sites through these embeds.

2. **Allow X (previously Twitter) embedded tweets:**
   - **Off:** Blocks embedded tweets, which can help prevent tracking by X but will also mean you won't see embedded tweet content on web pages.

3. **Allow LinkedIn embedded posts:**
   - **Off:** Remains off, continuing to block embedded LinkedIn content.

<img src="img/smb_after.png" alt="Brave Shield After">

### Benefits and Drawbacks

- **Benefits:** Blocking these embeds can significantly enhance your privacy by reducing the ways these social media platforms can track your activity across different websites.
- **Drawbacks:** Disabling these features means you won't be able to see or interact with social media content directly on websites, and you won't be able to use social media logins for quick access to services that support it.

By adjusting these settings according to your privacy preferences, you can balance between convenience and privacy.
</p>

<h3 align="center">2. Privacy and Security - Settings</h3>

# Explanation of Brave Privacy and Security Settings

***all the setting that i go over here are located here: brave://settings/privacy***

## WebRTC IP Handling Policy

WebRTC (Web Real-Time Communication) is a feature that enables voice and video communication directly within the browser without needing plugins. However, it can expose your IP address even when using a VPN. Brave offers different settings to manage how WebRTC handles IP addresses:

1. **Default:**
   - **Behavior:** Allows WebRTC to enumerate all interfaces, potentially exposing both public and private IP addresses.
   - **Best For:** Users who need seamless WebRTC functionality for tasks like video calls without concern for IP exposure.

2. **Default Public and Private Interfaces:**
   - **Behavior:** WebRTC uses the default route for HTTP connections, exposing associated private IP addresses.
   - **Best For:** Users who want some level of IP protection but still need WebRTC to function efficiently.

3. **Default Public Interface Only:**
   - **Behavior:** Limits WebRTC to using only the public interface route used by HTTP, not exposing local IP addresses.
   - **Best For:** Users who want better privacy without completely disabling WebRTC.

4. **Disable Non-Proxied UDP:**
   - **Behavior:** Forces WebRTC to use TCP instead of UDP, preventing local IP addresses from being exposed. This setting can effectively disable WebRTC if the proxy server doesn't support UDP.
   - **Best For:** Maximum privacy, suitable for users who prioritize security over the functionality of WebRTC.

**Best for Privacy and Security:** For the highest level of privacy, **"Disable Non-Proxied UDP"** is recommended. This setting ensures that WebRTC doesn't expose any local IP addresses, providing maximum protection against IP leaks.

## Other Privacy and Security Settings
### it's not recommended to disable the following settings as they impact your browsing security:

1. **Use Google Services for Push Messaging:**
   - **Off:** Disables push notifications that use Google's services, enhancing privacy by not relying on external notification services.

2. **Auto-redirect AMP Pages:**
   - **On:** Redirects AMP (Accelerated Mobile Pages) to their canonical (original) URLs, avoiding Google's AMP framework which can track user activity.

3. **Auto-redirect Tracking URLs:**
   - **On:** Bypasses tracking redirects, preventing websites from tracking your clickthrough behavior via URL redirects.

4. **Prevent sites from fingerprinting me based on my language preferences:**
   - **On:** Reduces the information sites can gather about your language settings, making it harder for them to create a unique fingerprint of your device.

5. **Send a "Do Not Track" request with your browsing traffic:**
   - **Off (by default):** Sends a request to websites asking them not to track you. Note that websites can choose to ignore this request.

These settings collectively enhance your browsing privacy by reducing the amount of data shared with external services and preventing various forms of tracking.



## Summary of Recommended Settings

For maximum privacy and security in Brave Browser, I recommend the following:

1. **WebRTC IP Handling Policy:** Set to "Disable Non-Proxied UDP"
   - This provides the highest level of protection against IP leaks through WebRTC.
2. **Other WebRTC settings:** Keep at their default values
   - Changing these may impact browser functionality without significant privacy gains.
3. **Additional Privacy Settings:** Enable as described in the "Other Privacy and Security Settings" section below
   - These settings enhance overall privacy without compromising basic browsing experience.

Remember, maximizing privacy may affect some website functionalities. Adjust settings based on your personal privacy needs and browsing habits.



## Note on "Do Not Track" Setting

The "Send a 'Do Not Track' request with your browsing traffic" setting deserves special consideration:

- **Default Setting:** Off
- **Recommendation:** Consider carefully before enabling

**Why you might want to keep it off:**

1. **Limited Effectiveness:** Many websites ignore or don't honor this request.
2. **Increased Fingerprinting Risk:** Paradoxically, enabling this setting can make your browser more uniquely identifiable (fingerprintable).
3. **Inconsistent Interpretation:** Websites may interpret and respond to this request differently:
   - Some might show non-personalized ads instead of targeted ones.
   - Others may still collect and use your browsing data for various purposes (e.g., security, content provision, analytics).

**Understanding "Do Not Track":**
- It's a request included with your browsing traffic.
- Its effect depends on whether and how websites respond to it.
- It doesn't prevent data collection by itself; it relies on the willingness of websites to honor the request.

**Bottom Line:** 
While the intent behind "Do Not Track" is privacy-focused, its practical impact is limited and it may unintentionally make your browser stand out. For most users, keeping this setting off and relying on Brave's other robust privacy features is likely the better choice for maintaining the best privacy online.

**Image for recommended settings for those wondering:**

<p align="center">
  <img src="img/recommend_ps_settings.png" alt="Brave Privacy and Security Settings">
</p>

# Tor Settings in Brave Browser vs Normal Tor Browser

## Tor Windows Settings in Brave

<p align="center">
  <img src="img/tor_default.png" alt="TOR mode on">
</p>

### 1. Private Window with Tor

- **What it does:** Opens a private browsing window that uses the Tor network to hide your IP address from the sites you visit.
- **Pros:**
  - Enhanced privacy by masking your IP address.
  - Access to onion services and websites blocked in your region.
- **Cons:**
  - Slower browsing speeds due to routing through multiple Tor nodes.
  - Some websites may not work correctly due to IP address changes.
- **Recommendation:** While this offers additional privacy, it's not as robust as the dedicated Tor Browser, which provides more comprehensive protection and anonymity.

### 2. Only Resolve .onion Addresses in Tor Windows

- **What it does:** Restricts access to .onion sites to Tor windows only.
- **Pros:**
  - Prevents accidental access to onion sites in non-Tor windows, which could compromise privacy.
- **Cons:**
  - Limits the ability to access .onion sites without opening a Tor window.
- **Recommendation:** Useful for ensuring that onion sites are accessed securely through Tor.

### 3. Volunteer to Help Others Connect to the Tor Network

- **What it does:** Enables the Snowflake extension, allowing users in censored countries to connect to the Tor network through your connection.
- **Pros:**
  - Helps support the Tor network and users in restricted regions.
  - Enhances the robustness and accessibility of the Tor network.
- **Cons:**
  - Uses some of your bandwidth to relay traffic.
  - Potential minor impact on your internet speed.
- **Recommendation:** Beneficial for those who want to support internet freedom and have sufficient bandwidth.

### 4. Use Bridges

- **What it does:** Allows the use of Tor bridges to connect to the Tor network in regions where it is blocked.
- **Pros:**
  - Provides access to Tor in censored regions.
  - Enhances the ability to bypass government or ISP blocks on Tor.
- **Cons:**
  - May require additional configuration.
  - Some bridges might be slower or less reliable.
- **Recommendation:** Essential for users in regions with heavy censorship; useful to have this option available.

## Why Tor Mode in Brave is Not Recommended Over the Normal Tor Browser

### Tor Mode in Brave:
- **Integration:** Tor mode in Brave offers easy access to Tor within the Brave browser.
- **Convenience:** Convenient for users who want occasional anonymity without switching browsers.
- **Limitations:** Provides basic Tor functionalities but lacks the full suite of privacy features available in the Tor Browser.

### Normal Tor Browser:
- **Comprehensive Privacy:** Designed specifically for anonymity, providing robust privacy protections.
- **Security Features:** Includes additional security measures such as NoScript, which prevents JavaScript exploits.
- **Updates:** Regular updates directly from the Tor Project to address vulnerabilities and enhance security.
- **Community Support:** Extensive support and documentation from the Tor community for troubleshooting and advanced configurations.

## Conclusion

- **Best for Maximum Privacy:** Use the Tor Browser for the most secure and private browsing experience.
- **Best for Convenience:** Use Tor mode in Brave for occasional private browsing with easy access to both Tor and regular websites.

## Summary

- Brave offers Tor integration for enhanced privacy, but it's not as comprehensive as the dedicated Tor Browser.
- Key Brave Tor settings include Private Window with Tor, .onion address resolution, and options to support the Tor network.
- While convenient, Brave's Tor mode lacks some advanced privacy features of the normal Tor Browser.
- For maximum privacy and anonymity, the dedicated Tor Browser is recommended.
- Use Brave's Tor features for occasional private browsing when convenience is preferred over maximum security.

*I just turn TOR mode off completely as it's not as secure as the normal TOR browser.*

<p align="center">
  <img src="img/tor_disabled.png" alt="TOR mode off">
</p>

## Data Collection Settings

When hardening Brave for maximum privacy, disable the following settings:

1. Allow privacy-preserving product analytics (P3A)
2. Automatically send daily usage ping to Brave
3. Automatically send diagnostic reports

Although these collect anonymous data to improve Brave, disabling them ensures no data is sent back to Brave servers, enhancing privacy.

<p align="center">
  <img src="img/tel_def.png" alt="Default Telemtry Settings">
</p>

**Recommendation:** Turn OFF all data collection settings for the highest level of privacy when hardening Brave.

<p align="center">
  <img src="img/tel_dis.png" alt="Disabled Telemtry Settings">
</p>

<hr>

<h4>brave://settings/security</h4>

### Safe Browsing

#### **Safe Browsing:**
- **Standard Protection:**
  - **Function:** Protects against dangerous websites, downloads, and extensions by checking them against a database of known threats. When a page looks suspicious, some data is sent to Google's Safe Browsing to verify its safety.
  - **Why It's Important:** Disabling Safe Browsing removes a crucial layer of protection against malware, phishing attacks, and other online threats, leaving you vulnerable to malicious content.

#### **Default Settings (OS Default):**
- **Function:** Uses the DNS (Domain Name System) resolver set by your operating system or network provider.
- **Pros:** Simple and reliable, uses existing system settings without additional configuration.
- **Cons:** May not provide the best privacy, as ISPs (Internet Service Providers) can log and monitor your DNS queries.

<p align="center">
  <img src="img/os_def_dns.png" alt="Default DNS">
</p>

#### **Custom Settings (Using Mullvad DNS):**
- **Function:** Configured to use Mullvad DNS (https://base.dns.mullvad.net/dns-query), a privacy-focused DNS service.
- **Pros:** Enhances privacy by using a DNS provider that does not log your DNS queries or track your browsing activity.
- **Cons:** Requires manual configuration.

<p align="center">
  <img src="img/my_dns_settings.png" alt="Mullvad DNS">
</p>

### Secure DNS

#### **Secure DNS:**
- **What It Does:** Encrypts DNS queries, preventing third parties from seeing which websites you visit. This is done by using protocols like DNS over HTTPS (DoH) or DNS over TLS (DoT).
- **Importance:**
  - **Privacy:** Protects against eavesdropping and manipulation of DNS data by ensuring that your DNS requests are encrypted and secure.
  - **Security:** Reduces the risk of DNS spoofing attacks, where attackers redirect you to malicious sites by altering DNS responses.

### Summary
- **Safe Browsing:** Essential for security; should remain enabled to protect against online threats.
- **Default DNS Settings:** Convenient but may compromise privacy.
- **Custom DNS (Mullvad):** Offers enhanced privacy and security by using a DNS provider that respects user privacy.
- **Secure DNS:** Crucial for maintaining privacy and security online by encrypting DNS queries and protecting against various attacks.
<hr>

# V8 Optimizer in Brave Browser
***brave://settings/content/v8***
#### **What is the V8 Engine?**
The V8 engine is an open-source JavaScript engine developed by Google, which is used in both Google Chrome and Brave browsers. It is responsible for executing JavaScript code in the browser, allowing websites to perform dynamic actions and interact with users. V8 compiles JavaScript directly to native machine code before executing it, which makes it very fast.

#### **V8 Optimizer:**
- **Default Behavior:**
  - **Sites Can Use the V8 Optimizer:** This setting allows the V8 engine to optimize JavaScript execution, which can significantly improve site performance and speed. It ensures that features using JavaScript work as intended.
  - **Don't Allow Sites to Use the V8 Optimizer:** Disabling this can reduce performance but makes the V8 engine more resistant to certain types of attacks, potentially increasing security.

#### **Customizing V8 Optimizer Behavior:**
- **Blacklisting Sites (Not Allowed to Use V8 Optimizer):**
  - You can add specific websites to a blacklist to prevent them from using the V8 optimizer. This might be useful for sites where you suspect the JavaScript could be malicious or where you experience performance issues that could be related to V8 optimizations.
  - **How to Add:** Click the "Add" button under "Not allowed to use V8 optimizer" and enter the URLs of the sites you want to restrict.

- **Whitelisting Sites (Always Allowed to Use V8 Optimizer):**
  - You can also add specific websites to a whitelist to ensure they always benefit from V8 optimizations, even if you generally prefer to restrict this feature.
  - **How to Add:** Click the "Add" button under "Always allowed to use V8 optimizer" and enter the URLs of the sites you want to allow.

### Summary
- **V8 Engine:** A high-performance JavaScript engine that enhances the speed and functionality of web applications.
- **V8 Optimizer:** Improves site performance by optimizing JavaScript execution. You can control its usage:
  - **Default Behavior:** Generally recommended for better performance.
  - **Custom Behavior:** Allows for specific sites to be blacklisted or whitelisted based on your preferences for performance and security.

*I personally keep it as default:*
<p align="center">
  <img src="img/v8.png" alt="V8 Engine">
</p>
<hr>

### Privacy and Security: Delete Browsing Data
*brave://settings/clearBrowserData*
#### **Delete Browsing Data**
- **Purpose:** Helps maintain your privacy by removing history, cookies, cache, and other browsing data.
- **Recommendation:** Regularly clear your cookies and cache to enhance privacy and security. This can prevent tracking and free up space on your device.
- **Customization:** You can customize what data to delete (e.g., browsing history, download history, cookies, cached images and files, passwords, and more) based on your preferences.

Clearing your browsing data periodically helps protect your privacy and keeps your browser running smoothly.

<p align="center">
  <img src="img/del_data.png" alt="Clear Browsing Data">
</p>

<hr>

### Site and Shields Settings in Brave

*brave://settings/content*

#### **Overview:**
These settings allow you to control what permissions and content sites can access and display, enhancing your privacy and security.


<p align="center">
  <img src="img/content1.png" alt="Settings content 1">
</p>

<p align="center">
  <img src="img/content2.png" alt="Settings content 2">
</p>

#### **Key Settings:**

1. **Location:**
   - **Default:** Don't allow sites to see your location.
   - **Why:** Prevents sites from tracking your physical location, which enhances your privacy.
   - **Recommendation:** Enable location access only for trusted sites that need it for functionality, like maps services.

2. **Camera:**
   - **Default:** Don't allow sites to use your camera.
   - **Why:** Protects against unauthorized access to your camera, which could be exploited for surveillance or spying.
   - **Recommendation:** Enable camera access only for sites where it's essential, such as video conferencing platforms.

3. **Microphone:**
   - **Default:** Don't allow sites to use your microphone.
   - **Why:** Prevents unauthorized listening, protecting your conversations from being intercepted.
   - **Recommendation:** Enable microphone access only for sites where it's necessary, like online meetings.

4. **Notifications:**
   - **Default:** Don't allow sites to send notifications.
   - **Why:** Avoids unsolicited notifications that can be intrusive and annoying.
   - **Recommendation:** Enable notifications only for sites where you want real-time updates.

5. **Block Cookies:**
   - **Default:** Third-party cookies are blocked.
   - **Why:** Reduces tracking by advertisers and improves privacy by preventing third parties from storing cookies on your device.
   - **Recommendation:** Keep this setting to block third-party cookies by default.

6. **JavaScript:**
   - **Default:** Sites can use JavaScript.
   - **Why:** JavaScript is necessary for many modern web functionalities, but it can also be used for malicious purposes.
   - **Recommendation:** Disable JavaScript for untrusted sites, but keep it enabled for trusted sites that require it.

7. **Images:**
   - **Default:** Sites can show images.
   - **Why:** Images are generally safe and necessary for a full web experience.
   - **Recommendation:** Keep this enabled, but disable for specific sites if needed.

8. **Pop-ups and Redirects:**
   - **Default:** Don't allow sites to send pop-ups or use redirects.
   - **Why:** Pop-ups and redirects can be used for phishing, ads, or malicious content.
   - **Recommendation:** Keep this setting enabled to block pop-ups and redirects, allowing exceptions only for trusted sites.

9. **Automatically Remove Permissions from Unused Sites:**
   - **Default:** Enabled.
   - **Why:** This removes permissions from sites you haven't visited recently, enhancing your privacy by limiting persistent access.
   - **Recommendation:** Keep this enabled for better privacy management.

### Why Default Denial is Important:
- **Security:** Prevents unauthorized access to sensitive features like your camera, microphone, and location.
- **Privacy:** Limits the ability of sites to track your activities and collect data.
- **Control:** Gives you the ability to grant permissions only to trusted sites, reducing the risk of exploitation.

### Conclusion
Keeping these permissions disabled by default and whitelisting only necessary and trusted sites is a crucial step in maintaining robust privacy and security while browsing.
<hr>

<h3 align="center">3. Autofill and passwords - Settings</h3>


### Autofill and Passwords: Why You Should Use a Dedicated Password Manager

#### **Built-in Autofill Features:**
- **Convenience:** Built-in browser autofill features, like those in Brave, provide an easy way to save and automatically fill passwords, payment methods, and addresses.
- **Security Concerns:** These built-in features, while convenient, are not as secure as dedicated password managers. They are more vulnerable to browser exploits and attacks that could expose your sensitive information.

#### **Why Choose a Dedicated Password Manager like Bitwarden:**

1. **Enhanced Security:**
   - **Encryption:** Dedicated password managers use robust encryption to protect your data. Bitwarden, for instance, uses end-to-end encryption, ensuring that only you can access your stored information.
   - **Security Audits:** Bitwarden undergoes regular security audits to ensure its platform remains secure and free from vulnerabilities.

2. **Cross-Platform Syncing:**
   - **Seamless Access:** Bitwarden allows you to access your passwords and other data across multiple devices and platforms securely, including mobile devices, desktops, and web browsers.

3. **Advanced Features:**
   - **Two-Factor Authentication (2FA):** Provides an additional layer of security for accessing your password vault.
   - **Password Generator:** Generates strong, unique passwords for each of your accounts, reducing the risk of password reuse and improving security.
   - **Security Reports:** Bitwarden can provide reports on the strength of your passwords and alert you to potential security issues like reused or weak passwords.

4. **Privacy:**
   - **Data Ownership:** With services like Bitwarden, you maintain ownership and control over your data. They have a strong privacy policy that ensures your data is not monetized or shared without your consent.

5. **Community Trust:**
   - **Open Source:** Bitwarden is open-source software, meaning its code is publicly available for review. This transparency helps build trust and allows security experts to inspect the code for vulnerabilities.

### Summary
Using a dedicated password manager like Bitwarden offers superior security, better cross-platform functionality, and enhanced privacy features compared to built-in browser autofill solutions. For the best protection of your sensitive data, it is recommended to use a dedicated password manager.

*brave://settings/autofill*

<p align="center">
  <img src="img/autofill.png" alt="Disable Autofill">
</p>

*brave://settings/addresses*

<p align="center">
  <img src="img/add.png" alt="Disable Address Autofill">
</p>

*brave://password-manager/settings*

<p align="center">
  <img src="img/pass.png" alt="Disable Password Autofill">
</p>

*brave://settings/payments*

<p align="center">
  <img src="img/pay.png" alt="Disable payment and autofill">
</p>

<hr>

<h3 align="center">4. Extensions - Settings</h3>


*brave://settings/extensions*

<p align="center">
  <img src="img/ext_def.png" alt="Default Extension Settings">
</p>

#### **Manifest V2 Extensions**

- **What is Manifest V2?**
  - Manifest V2 is a format for writing extensions for browsers like Chrome and Brave. It allows developers to specify permissions, background scripts, and other features needed by the extension.
  - **Brave Shields and Manifest V3:** Brave's ad and tracker blocking technology, Brave Shields, is built directly into the browser. This means that changes in extension manifests, such as the transition from Manifest V2 to Manifest V3, do not affect Brave Shields' functionality. Brave Shields will continue to block ads and trackers regardless of these changes.

#### **Hangouts**
- **Hangout Component:** Uses the Hangouts component to enable screen sharing and other features.
- **Controversy:** Google Hangouts has faced various privacy concerns and will be phased out by Brave. This change reflects Brave's commitment to enhancing user privacy and security.
  - **Brave's Action:** Brave is actively working to remove Hangouts from its components due to its discontinuation and privacy issues.

    *See more here:* https://github.com/brave/brave-core/pull/24594

#### **Enabled Settings:**
1. **Media Router:**
   - **Function:** Enables casting features in the browser.
   - **Recommendation:** Keep this enabled if you use devices like Chromecast to cast content from your browser to your TV or other devices. Disable if you do not use casting features to reduce potential attack vectors.

2. **WebTorrent:**
   - **Function:** Allows torrents to be displayed directly in the browser.
   - **Recommendation:** Keep this enabled if you frequently download torrents. Disable if you do not use torrents to minimize potential security risks.

#### **Disabled Settings (by default):**
1. **Allow Google login for extensions:**
   - **Recommendation:** Keep this disabled to avoid using Google services for logging into extensions. This can enhance privacy by reducing the data shared with Google.

2. **Widevine:**
   - **Function:** Digital Rights Management (DRM) component for viewing protected streaming video.
   - **Recommendation:** Enable only if you need to access DRM-protected content such as certain streaming services. Keeping it disabled can enhance privacy.

### Summary
- **Manifest V2 Extensions:** These will not affect Brave Shields, ensuring continuous protection against ads and trackers.
- **Hangouts Removal:** Brave is removing the Hangouts component.


- **Extension Settings:**
  - Enable Media Router and WebTorrent if you use casting and torrenting features.
  - Keep settings like Google login for extensions and Widevine disabled unless necessary to enhance privacy and security.

*These are my extension settings:*
<p align="center">
  <img src="img/ext_my.png" alt="My Extension Settings">
</p>

<hr>

<h3 align="center">5. Search - Settings</h3>

*brave://settings/search*



***default search settings:***
<p align="center">
  <img src="img/def_search.png" alt="Default Search Settings">
</p>

**Here's a concise list of what The Web Discovery Project is:**

• The Web Discovery Project is an opt-out feature that allows users to contribute anonymous data to improve Brave Search's relevance and independence.

• Data collected includes search queries, clicked results, visited URLs, time spent on pages, and page metadata, but cannot be linked back to individual users.

• The project uses privacy-preserving methods like unlinkability and distributed quorum to protect user anonymity.

• Collected data helps Brave understand popular keywords, relevant websites, and user interactions to improve search results.

• Users can opt out at any time, and the data retention period is one year.

• The project has minimal performance impact and runs only on desktop devices.

*More info can be found here:* https://support.brave.com/hc/en-us/articles/4409406835469-What-is-the-Web-Discovery-Project

***(Hardened) Search Engine Settings:***

<p align="center">
  <img src="img/rec_search.png" alt="My Search Settings">
</p>

<hr>

<h3 align="center">5. Wallet/Crypto - Settings</h3>

*brave://settings/web3*

**These are the default settings except for "Automatically lock Brave Wallet" which is set by default to 10 min**
<p align="center">
  <img src="img/wallet1.png" alt="Wallet Settings 1">
</p>


<p align="center">
  <img src="img/wallet2.png" alt="Wallet Settings 2">
</p>

**I highly recommend you give Brave wallet a try, we are waiting for on-chain rewards to be implemented**

*see more here:* https://brave.com/blog/rewards-solana/

**if you decide to disable the wallet here is how you can fully disable it:**


<p align="center">
  <img src="img/wallet_dis1.png" alt="Wallet Settings Disabled 1">
</p>

<p align="center">
  <img src="img/wallet_dis2.png" alt="Wallet Settings Disabled 2">
</p>



<p align="center">
  <img src="dis_sponsored_images.png" alt="Disable Sponsored images">
</p>


<p align="center">
  <img src="img/hide_cards.png" alt="Hide cards">
</p>

*brave://settings/appearance*
<p align="center">
  <img src="img/hide_br_bw.png" alt="Hide wallet and Rewards">
</p>

































***If you find any errors in this guide pls let me know
I will change it ASAP***

# Begging sections

If you liked this guide and want to help with my orange juice addiction you can donate here:


***Monero***
<p align="center">
    <img src="img/monero_qr.jpg" alt="Monero" width="512px" height="512px">
</p>

```
47E2j1R4HrCcvV75mNo5DRRmSQcmi9rgKSFkd1o4HbshXx5NCiHu7zsFy7AgiWrEZrZ2o1aLdfNeJPD74y6RNCVC9LvgnnD
```

***Bitcoin***
<p align="center">
    <img src="img/bitcoin_qr.png" alt="Bitcoin" width="512px" height="512px">
</p>
    
```
bc1q3zsfj3k0utdkm725rg43vhu3syw0x5va8mzspm
```

***Ethereum***
<p align="center">
    <img src="img/ethereum_qr.png" alt="Ethereum" width="512px" height="512px">
</p>
    
```
0xc8803D45ADE7c869bC3b15206e81fB47Bb0A44D8
```


***Basic attention token***
<p align="center">
    <img src="img/ethereum_qr.png" alt="BAT" width="512px" height="512px">
</p>
        
```
0xc8803D45ADE7c869bC3b15206e81fB47Bb0A44D8
```