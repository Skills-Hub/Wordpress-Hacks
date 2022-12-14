## Top wordpress issues 
### 3. 404 Not Found
A 404 error occurs when a user attempts to access a web page that doesn’t exist. Instead of finding the resource they were looking for, they’ll see a page similar to this one:

This problem is relatively harmless but nevertheless frustrating for users. To avoid it, make sure to fix broken links on your site periodically and implement redirects if you delete a page or move it to a new URL.

### 4. 405 Method Not Allowed
The 405 Method Not Allowed error is your server’s way of saying that it has received the browser’s request but rejected it for some reason.

There are several possible ways to resolve this problem, including rolling back recent theme and plugin updates, checking your server’s configuration and error logs, and debugging your application code.

### 5. 413 Request Entity Too Large
If this error appears in your browser, it means that the server of the site you’re trying to access can’t process the HTTP request you’ve made because it’s too large.

This often occurs if you’re trying to upload a very ‘weighty’ file. You can resolve this problem by increasing your maximum HTTP request size.

100+ Most Common WordPress Errors and How to Fix Them

### 6. 429 Too Many Requests
If a user attempts to access a certain resource too many times over a short span of time, they may receive a 429 Too Many Requests error. This is your server’s way of blocking out suspicious behavior.

To help prevent cyberattacks on your login page that may lead to a 429 error, you can change its default URL. Other solutions include testing for theme and plugin conflicts.

500 Errors
Any error on your site that is labeled with a number between 500 and 599 is an indication that your server is incapable of performing a given request for some reason. Here are a few of the most common examples.

### 7. 500 Internal Server Error
In addition to preventing users from accessing your site, a 500 Internal Server Error can negatively impact your SEO if not resolved quickly:

Unfortunately, the 500 error has many possible causes and solutions, which can make troubleshooting this issue tricky. You can start by clearing your browser cache and reloading the page. If that doesn’t work, you can dive into more technical debugging methods.

8. 501 Not Implemented
This error means that your server doesn’t have the functionality needed to complete the request made by the user’s browser. It’s likely that the server doesn’t recognize the request method.

As with a 500 Internal Service Error, a 501 error can lower your search engine rankings if you don’t resolve it within a few hours. You can try reloading the page, clearing the browser cache, and disabling any active proxy settings to resolve it.

However, you’ll likely need to contact your host for help.

9. 502 Bad Gateway
In cases where one server is acting as a proxy or ‘gateway’ for another, there’s a chance that users may encounter a 502 Bad Gateway error. This occurs when the proxy receives an invalid response from the inbound server.

A 502 error can impact your SEO, so it’s best to get it cleared up fast. Reloading the page and clearing your browser cache are good places to start. If those solutions don’t work, check for issues with your DNS, try disabling your CDN or firewall, or contact your host for assistance.

10. 503 Service Unavailable
When a 503 Service Unavailable error appears, it means that for some reason your server can’t be reached. Although your website is up, it won’t be accessible to users.

This may be due to routine maintenance, high traffic levels, or a more serious problem with your server. The good news is that a 503 error won’t influence your search engine rankings. It can still be highly annoying to visitors, however. To fix it, you can try:

Deactivating your plugins.
Switching to a default theme.
Disabling your CDN.
Limiting the WordPress Heartbeat API.
Increasing your server’s resources.
Enabling WP_DEBUG.
If none of these solutions work, your best course of action is to get in touch with your host’s support team.

100+ Most Common WordPress Errors and How to Fix Them

11. 504 Gateway Timeout
Like a 502 error, the 504 Gateway Timeout response is the result of a problem with the communication between an inbound server and a proxy. Essentially, it means that the latter server timed out while waiting for the former to respond to a request.

This type of error can negatively affect your SEO. Possible solutions include reloading the page, disabling any active proxy settings, checking your DNS for issues, and temporarily disabling your CDN.

Server-Related Errors
Your server is responsible for storing all of your WordPress site’s files and communicating with browsers to make your content available to users.

While the 400 and 500 errors already listed involve your server in some way, there are also some more WordPress-specific issues that can be caused by problems with your server.

12. WordPress Memory Limit Error
Your hosting provider allocates a certain amount of server memory to your site. In the event that you reach your server’s memory limit, you may run into issues installing a new plugin or theme, or uploading media files to your site.

Instead of successfully adding your new resource, you’ll see a message that reads: “fatal error: allowed memory size has been exhausted”. If this happens, you can try increasing your PHP memory limit by editing your wp-config.php file.

Alternatively, you could check how much disk space you’re using, see if you can improve your PHP memory limit, and consider upgrading to a new hosting plan that offers more space for your growing WordPress site.

13. Uploaded File Exceeds the upload_max_filesize Directive in php.ini
On a similar note, your host also sets a limit on the maximum size for individual files that you can upload to your server. You can see this limit by navigating to Media > Add New in your WordPress dashboard and looking for the Maximum upload file size (the default upload size at Kinsta is 128 MB):



If you need to upload a file that is larger than the specified maximum size, you can change the limit by editing your php.ini file. Alternatively, you can contact your hosting provider to discuss the issue with them.

This is far simpler and less risky than trying to change it yourself and shouldn’t be an issue for your host’s support team.

14. Fatal Error: Maximum Execution Time Exceeded
Servers have time limits on how long scripts can run (usually 30 seconds, at Kinsta the default maximum execution time is 300 seconds). In the event that a PHP script on your WordPress site takes longer than the allotted time limit, you’ll likely see the message: “fatal error: maximum execution time exceeded”.

You can resolve this issue by increasing your site’s execution time limit. To do so, you’ll need to find the script that is running too long,  which is likely part of a plugin or theme and remove it.

15. Upload: Failed to Write File to Disk
Adding images to your posts and pages can make them more useful, and interesting, and drive additional organic traffic. However, you’ll have a difficult time doing this if you see a message like “Upload: Failed to write file to disk” whenever you try to add media files to your site.

This error is often due to incorrect file permissions. You can fix this problem by changing your file permissions via File Transfer Protocol (FTP).

However, it can also be an issue with your server. When you upload files to WordPress, they are first saved to a temporary folder on your server. Then, they are moved to the appropriate WordPress directory. If changing your file permissions doesn’t fix this error, contact your host and ask them to empty your temporary files directory, as it may be full and prevent uploads.

100+ Most Common WordPress Errors and How to Fix Them

16. Secure Connection Error
When you update your WordPress installation’s core files, your site has to connect to WordPress.org. Sometimes, due to your server’s configuration, this isn’t possible. The result is a warning in your WordPress dashboard.

As this is a problem directly related to your server, you’ll likely need to contact your host in order to resolve it. Your server may be under a DDoS attack, in which case the error should resolve on its own shortly. Alternatively, you can try fixing the problem yourself by pointing your server towards WordPress.org through Secure Shell Protocol (SSH).

Security-Related Errors
Implementing WordPress security best practices on your site is wise. Cyberattacks could cause serious damage that requires a lot of money to fix. Unfortunately, sometimes the measures you put in place to protect your site can lead to errors.

Info

If you host your site at Kinsta, we offer a hack fix guarantee and will clean your site of malware for free.

17. Cloudflare Error 521
Although this is a 500 error like the ones we described in the previous section, it’s specific to Cloudflare. This popular platform is used as a CDN, and for protection against DDoS and other attacks.

Seeing a 521 error on your site means that Cloudflare can’t connect to your server. Either it’s down or is blocking the service for some reason. Generally speaking, checking to make sure your server is up and that its firewall has all of Cloudflare’s IP ranges whitelisted will let you know what’s causing the problem. You can then take steps to work with your host and resolve it.

Suggested reading: How to Set up Cloudflare APO for WordPress.

18. “Sorry, This File Type Is Not Permitted for Security Reasons”
As a security measure, WordPress has a standard list of permitted file types. This prevents malicious parties from adding executable files to your site that could compromise users’ sensitive information.

If a user tries to upload a file type that is not on that list, they’ll see a message reading: “Sorry, this file type is not permitted for security reasons”:

ou can enable uploads of file types not allowed in WordPress’ default settings by editing your wp-config.php file.

The WP Extra File Types plugin can also be used as an alternative solution.

19. “Sorry, You Are Not Allowed to Access This Page”
We briefly touched upon file permissions earlier in this post, but to recap, they determine who can edit which files on your WordPress site. This keeps your website safe from hackers who might want to insert malicious code.

However, if your permissions settings are incorrect, they could inadvertently block you or well-meaning users from accessing your site.

This can result in an error that reads: “Sorry, you are not allowed to access this page”.

There are many possible solutions to this issue. You may want to try:

Resetting your file permissions via Secure File Transfer Protocol (SFTP).
Check to make sure your account is assigned the correct user role via phpMyAdmin.
Ensuring that your database prefix is correct.
Troubleshooting for plugin and theme conflicts.
In the worst-case scenario, you can also restore a backup of your site or reset WordPress.

100+ Most Common WordPress Errors and How to Fix Them

20. “Installation Failed: Could Not Create Directory”
Whenever you install a plugin or theme on your WordPress site, its files are added to your server. If during an installation or update you receive a message that says “Installation failed: Could not create directory”, it means that for some reason, WordPress was unable to add the necessary files to your server.

The same applies to plugin and theme updates. This is another file permissions-related error.

To fix it, make sure you’re allowed to Write in your wp-admin, wp-content, and wp-includes directories via FTP.

21. Incorrect File Permissions
In addition to denying you access to certain areas of your site, as in the case of the “Sorry, you are not allowed to access this page” error, incorrect file permissions can prevent you from:

Updating or installing plugins and themes.
Publishing or updating posts and pages.
Uploading images.
On the other hand, if your file permissions aren’t too strong, you leave your website vulnerable and run the risk of hackers gaining access to your files. There they can delete content, steal data, or add their own malicious code.

If you’re running into one of the above issues, or suspect that you’ve been hacked, you may want to verify your file permissions via SFTP:

The default numeric values for WordPress are 755 for folders and 644 for files.

22. ERR_SSL_PROTOCOL_ERROR
Secure Sockets Layer (SSL) certificates are a security measure used to encrypt data. This prevents hackers from stealing sensitive data such as credit card information as it’s transferred between servers.

If you’ve recently switched hosting providers or installed a new SSL certificate on your site, you may see an ERR_SSL_PROTOCOL_ERROR in your browser. This means that, for some reason, your server was unable to establish a secure connection.

There are several steps you can take to resolve this issue, including updating your browser and operating system, verifying your SSL certificate, disabling browser extensions, and clearing your browser cache and cookies.

100+ Most Common WordPress Errors and How to Fix Them

23. ERR_SSL_VERSION_OR_CIPHER_MISMATCH
The ERR_SSL_VERSION_OR_CIPHER_MISMATCH error could indicate that your browser or operating system is out of date. It may also result from issues with your SSL certificate, or pop up after you migrate your WordPress site to a new host.

If updating your browser and the operating system doesn’t help, check for a name mismatch in your SSL certificate. Alternatively, clearing your computer’s SSL state may resolve the issue, or your SSL certificate may be outdated.

24. Mixed Content Warnings
When you add an SSL certificate to your WordPress site, it will start running HTTPS instead of HTTP. In the event that your website is trying to load both HTTPS and HTTP content or scripts simultaneously, you’ll see a mixed content warning.

This will probably read as some variation of: “This site is not fully secure”. In order to resolve the error, you’ll need to follow a few steps to determine which HTTP resources are loading and remove or replace them with HTTPS resources.

25. SSL Handshake Failed
This SSL connection-related error occurs when the browser cannot establish a secure connection with the server. Unfortunately, this can happen for various reasons. You can read more about it here: “How to Fix the “SSL Handshake Failed” Error (5 Methods)“.

100+ Most Common WordPress Errors and How to Fix Them

WordPress Media Errors
In the world of WordPress, ‘media’ most often refers to image files. However, it also includes video and audio. While these elements can provide engaging and interesting content for your users, they’re sometimes tricky to incorporate due to various errors that may arise in the process.

26. WordPress HTTP Error (Uploading Image to the Media Library)
While trying to upload a file to the WordPress Media Library, you may have come across a vague ‘HTTP error’. This generally appears as a small popup box on the right side of the image uploader.

There are a few possible causes for this problem, including an expired login session, disallowed characters in the file name, wrong permission, and server-side issues.

First, start by refreshing the page. If that doesn’t work, try resizing or renaming your media file. If not in luck, you should then check your permissions or temporarily deactivate your plugins and theme. In the event that you still can’t complete your upload, you may want to contact your host.

100+ Most Common WordPress Errors and How to Fix Them

27. The Add Media Button Isn’t Working
In the WordPress Classic Editor, the Add Media button is an important feature:

This button enables you to quickly upload new media files or select one from your Media Library to add to your post. However, sometimes clicking on the button does nothing or it may be missing from the editor entirely.

If this is the case, the issue is likely due to a plugin or theme conflict. You can resolve it by adding the define(‘CONCATENATE_SCRIPTS’, false) function to your wp-config.php file or by troubleshooting for potential compatibility errors.

28. Broken Media Files
If you open your media library and find that all of your images are gone entirely or have been replaced with placeholders, your files may be ‘broken’:

This can happen for a wide variety of reasons, including:

A problem with your server, such as a performance issue.
Compatibility errors between your plugins and/or theme.
Incorrect file permissions.
A hack or other attack.
To fix the issue, you can try resetting the file permissions for your uploads directory to 755. If that doesn’t work, look to see if there may be any plugin conflicts. After that, if your images are still broken, contact your hosting provider to see if the cause is a server issue.

100+ Most Common WordPress Errors and How to Fix Them

29. “There Has Been an Error Cropping Your Image”
In the WordPress Media Library, you can implement minor edits to the images you’ve uploaded, such as rotations and cropping. While attempting to edit in this way, you may receive the message: “There has been an error cropping your image”.

There are two possible causes for this error. The first is that you’re running on an outdated version of PHP, in which case you can simply upgrade to fix it. On the other hand, your server may be missing the necessary Graphics Draw (GD) package.

If this is the case, you’ll need to follow the appropriate steps for installing it based on your setup. In the event that you run into trouble, you should contact your hosting provider for help.

30. Incorrect Facebook Thumbnail
Social sharing can be an efficient method for building your website’s audience. However, sometimes the wrong thumbnail image may be displayed when your posts are shared on Facebook.

This often occurs when multiple images in your post include the Open Graph (OG) tag. Facebook uses this tag to guess which image it’s supposed to use for the thumbnail, but when multiple images include it, the platform gets confused.

One way to fix this issue is by using Yoast SEO’s social sharing features. By setting your Facebook thumbnail via this plugin, you can ensure that the correct image has the OG tag in place.

100+ Most Common WordPress Errors and How to Fix Them

Database Errors
Your WordPress installation is made up of two key parts: its files and its database. While you’re more likely to interact with the former on a regular basis, your database is also vital to your site’s ability to function properly.

31. Error Establishing a Database Connection
In the event that your website can’t establish a connection with your MySQL database, it won’t be able to retrieve the data necessary to display your content. Instead, you’ll see an error like this one:



This will prevent users from viewing the front end of your site, and also locks you out of your WordPress dashboard. The most common cause of this error is that your database credentials are incorrect. You can change them in your wp-config.php file.

100+ Most Common WordPress Errors and How to Fix Them

32. The WordPress Database Is Corrupt
‘Corruption’ is a general term applied to WordPress databases and files when they’ve become compromised or unusable. This will often result in an Error Establishing a Database Connection.

Ideally, you’ll want to restore a backup of your database to replace the corrupt version. If that’s not possible, you can also fix this error by adding the define(‘WP_ALLOW_REPAIR’, true) function to your wp-config.php file.

Suggested reading: check out this guide on how to troubleshoot and repair WordPress database issues. You can also fix some of these issues by using a free WordPress database plugin.

PHP Errors
PHP is a coding language that is integral to WordPress. Issues related to its functionality can prevent you from editing your site or result in intrusive messages and notifications.

33. PHP Errors in WordPress
When there is a problem with your WordPress site’s PHP, you’ll see a message or warning at the top of your WordPress dashboard stating what the problem is and which files are affected.

These messages are intended for developers, so they can dig into their sites’ code and revise the issue. If you don’t have experience with PHP, trying to resolve these errors could cause more problems for your site.

In the event that this describes your situation, don’t worry. PHP errors shouldn’t stop your site from running or prevent users from accessing it.

Ideally, you’ll want to contact the developer of any related plugins or themes that might be causing the issue. Otherwise, you can hire a developer to help you fix it.

34. “Missing a Temporary Folder”
Any time you upload a file to your WordPress site, it’s first stored in a temporary folder before being moved to its permanent directory. However, incorrect PHP settings on your server could prevent access to this temporary folder, leading to an error on your WordPress site.

Resolving this problem requires you to access your server via FTP and add the following function to your wp-config.php file:

100+ Most Common WordPress Errors and How to Fix Them


100+ Most Common WordPress Errors and How to Fix Them
Then, you can add a new folder named temp to your wp-content directory.

WordPress File Errors
From your posts and pages to your plugins and themes, your WordPress installation contains hundreds if not thousands of files. Errors related to these key components can result in lost or unavailable content.

35. “Destination Folder Already Exists”
When you install a new theme or plugin on your WordPress site, a folder is created on your server to store its files. If you attempt to install a plugin or theme, and a folder with the same name is already saved on your server, you’ll see an error reading “Destination folder already exists…Plugin installation failed”:


100+ Most Common WordPress Errors and How to Fix Them
Your first step when confronted with this issue should be to check to see whether the plugin or theme is already installed.

If not, access your server via FTP and navigate to your wp-content folder. Then, look through your plugins or themes to see if a folder with the same name as the component you’re attempting to install exists. Once you delete that folder, you can try your installation again.

100+ Most Common WordPress Errors and How to Fix Them

36. The WordPress Theme Stylesheet Is Missing
CSS is a coding language that determines your site’s ‘styling’. This may include colors, fonts, and a variety of other elements that make your website interesting to look at.

When it comes to WordPress themes, all the necessary CSS is contained within a file called a ‘stylesheet’. If your theme’s stylesheet isn’t available, your site won’t be able to load properly, and you’ll see an error:


100+ Most Common WordPress Errors and How to Fix Them
This may also occur during a theme installation:

This could happen because your theme’s stylesheet hasn’t been uploaded to your server, or because it’s named incorrectly and therefore can’t be found. To fix the problem, access your server via FTP and navigate to your theme’s subdirectory.

Then, look for your theme’s stylesheet. If it’s not there, retrieve it from your theme’s files and upload it to your server. Make sure the file is named style.css and is saved within the correct theme folder.

100+ Most Common WordPress Errors and How to Fix Them

37. Pluggable.php File Errors
Your WordPress site’s pluggable.php file enables users, plugins, and themes to override core functionalities. If a plugin or theme isn’t coded properly, it may result in a conflict with this file.

The issue will appear as a PHP error message in your WordPress dashboard that references your pluggable.php file. However, the cause of the problem isn’t usually within pluggable.php itself, it could be your wp-config.php or functions.php for example.

Instead, you’ll need to find the reallocation of the conflict in the error message. Then, navigate to the relevant file and fix it by removing spaces, empty lines, or something similar.

38. WordPress Files Are Corrupt
Just as your WordPress database can become corrupt, so too can its files. This will make them inaccessible, which is a big problem, especially when it comes to core files.

Corrupt files may be the result of a server failure, incorrect file permissions, or a PHP version error. The simplest fix is to restore a site backup.

First, log in to the MyKinsta dashboard. Go to “Sites” on the left-hand side and then click on the WordPress site for which you need to restore a backup.

Pick your preferred backup option from those provided and click on the “Restore to” button to decide whether you want your WordPress site backup restored on your live or staging site.

You will then have to confirm the backup restoration by entering your site name. Then click on “Restore.” This will overwrite your live environment.

Alternatively, you can replace core files by downloading WordPress, deleting the corrupt files via FTP, and then uploading fresh copies from the WordPress .zip file.

100+ Most Common WordPress Errors and How to Fix Them

Browser Errors
Visitors access your website using browsers of their choosing. This means that various browser errors can keep users from reaching your site. Preventing them will help you avoid missing out on traffic.

39. “Not Secure” Warning in Chrome
When browsing the internet using Google Chrome, you may have noticed that some pages have a ‘Not Secure’ warning next to their URLs:

The browser displays this warning when a website is not using an SSL certificate. If your pages trigger these messages in users’ browsers, it can hurt your site’s credibility, and impact your traffic level, SEO, and conversion rates. To prevent this from happening, you can install an SSL certificate.

More recently, Chrome started showing ERR_SSL_OBSOLETE_VERSION warning messages for websites that aren’t using TLS 1.2 or 1.3.

100+ Most Common WordPress Errors and How to Fix Them

40. “Your Connection Is Not Private” Browser Error
Even worse than the “Not Secure” warning in Chrome is the “Your Connection Is Not Private” page. This error prevents users from easily accessing your site, due to a problem with its SSL certificate (or lack thereof).

If they encounter this page, users may be scared away from your site for fear of their personal information being stolen. You can try to prevent this from happening by ensuring that your SSL certificate is installed properly, but it may also be a client-side issue that your users will have to fix themselves.

41. ERR_TOO_MANY_REDIRECTS
A redirect loop, which often displays as “ERR_TOO_MANY_REDIRECTS”, happens when there’s a misconfiguration of redirects on your server.

For instance, this could mean that URL 1 is pointing to URL 2, but URL 2 is pointing back to URL 1, causing an infinite loop. Users can try fixing this error by deleting your site’s cookies and clearing their browser caches. You can also try to determine the nature of the redirect loop, in order to figure out the source of the problem and then resolve it.

42. ERR_CONNECTION_REFUSED
Like many browser issues, the ERR_CONNECTION_REFUSED issue usually isn’t caused by something specific to WordPress. However, if users contact you because they can’t access your site due to this message in Chrome, it still helps to be able to tell them how to fix the problem.

The ERR_CONNECTION_REFUSED error occurs because the user’s browser was unable to connect to your site’s server. This could be a server-side problem, in which case you should check to see if your site is down and contact your hosting provider. Alternatively, you can try instructing your users to restart their routers and clear their browser caches.

100+ Most Common WordPress Errors and How to Fix Them

43. ERR_EMPTY_RESPONSE
The ERR_EMPTY_RESPONSE issue occurs when a user’s browser sends a request to your site and your server sends nothing back. The most popular fixes for this issue are to clear your browser cache and reset your network settings.

You may also want to advise users who are experiencing this problem to disable any Chrome extensions they’re using and try temporarily disabling their anti-virus software.

100+ Most Common WordPress Errors and How to Fix Them

44. DNS_PROBE_FINISHED_NXDOMAIN Browser Error
Your DNS is the system that takes your website’s IP address and turns it into a readable domain, such as kinsta.com. If your DNS fails to translate your domain into your site’s IP address correctly, users will see the DNS_PROBE_FINSHED_NXDOMAIN browser error in Chrome.

The first steps to resolve this issue are to release and renew your IP address. If that doesn’t work, you may suggest that users try temporarily disabling their anti-virus software or Virtual Private Networks (VPNs).

Suggested reading: How to Fix the DNS_PROBE_FINISHED_BAD_CONFIG Error Code.

troubleshooting Miscellaneous WordPress Errors
While many WordPress errors can be traced back to a specific cause, some are a little more difficult to diagnose. They may have multiple possible origins or lead back to a minute detail that doesn’t seem significant.

Below are a variety of WordPress problems that don’t fit neatly into the categories we’ve covered so far.

45. The White Screen of Death
One of the most famous WordPress errors is the White Screen of Death (WSoD). It causes your site to display as a blank white page to its users. This issue may also lock you out of your WordPress dashboard. Usually, it is caused by a plugin compatibility issue.

The best course of action for resolving it is to find the plugin that’s causing the conflict and remove it. Other possible causes include syntax errors, reaching your site’s memory limit, and file permissions issues.

100+ Most Common WordPress Errors and How to Fix Them

46. Locked Out of the WordPress Admin Dashboard
Your WordPress dashboard is highly important for numerous tasks, including fixing many common WordPress errors. However, sometimes the issues you’re experiencing on your site can lock you out of your WordPress dashboard.

There are many possible causes for this problem. If you can, try to determine whether you’re locked out due to a separate problem, and then take steps to resolve the root of the issue. You can also try restoring a backup of your site, or disabling a security plugin via FTP if you believe it’s keeping you from your site’s backend.

47. Can’t Connect via SSH or SFTP
Sometimes, WordPress management or troubleshooting will require that you access your server directly. SFTP enables you to access your files (learn the difference between SFTP and FTP), and SSH permits a wide variety of other remote tasks (here’s a guide on how to get started with SSH).

If you’re attempting to use SFTP or SSH to reach your server but can’t connect, you may need to delete outdated IP addresses from your known_hosts file.

48. SSH Connection Refused
In the event that you’re trying to connect to your server via SSH, and you see a message that reads “Connection refused” in your command-line interface, the problem is slightly different:

Instead of editing known_hosts, you’ll need to check a few things related to your SSH configuration.

First, make sure that your server has an SSH daemon installed. You should also check your credentials and determine if the port you’re using is open. The issue could also be due to your firewall settings.

49. Briefly Unavailable for Scheduled Maintenance
Whenever you run updates on your WordPress site, it temporarily goes into maintenance mode. During this time, anyone who tries to access your site will see a message that says something like: “Briefly unavailable for scheduled maintenance. Check back in a minute”:

This isn’t truly an error, since it’s supposed to happen, but users may interpret it differently. If they contact you about it but you’re not experiencing trouble on your end, you’ll want to recommend that they reload the page.

If you’re seeing this message while running updates in WordPress, on the other hand, your site may have gotten stuck in maintenance mode.

100+ Most Common WordPress Errors and How to Fix Them

50. WordPress Stuck in Maintenance Mode
Closing your browser in the middle of an update or running bulk plugin updates can cause your site to get stuck in maintenance mode. In this case, you’ll see the same message that users see on the front end when you run updates.

Fortunately, fixing this problem is quite simple. All you have to do is access your site’s files via FTP, and delete the one named .maintenance:



After that, you can check back with your site and all should be well again.

51. Changes Aren’t Visible on Your Live Site
If you’ve put in a lot of hard work to make updates to your site, only to check the front and see that none of them are visible, you may be feeling frustrated. The good news is that this problem is usually very simple to fix.

Most often, it’s the result of a caching issue. First, you can try clearing your browser cache. If your changes still aren’t visible and you’re using a caching plugin, check its documentation to learn how to clear the plugin’s cache as well.

100+ Most Common WordPress Errors and How to Fix Them

52. Missed Schedule
A consistent upload schedule is part of a strong content strategy. WordPress helps with this by enabling you to schedule posts for publication at specific dates and times.

Unfortunately, it doesn’t always work as intended, resulting in missed schedule errors. Generally speaking, the quickest solutions to this problem are either available via plugins, such as Scheduled Post Trigger or WP Scheduled Posts Pro, or by editing cron jobs.

Here at Kinsta, we configure your WordPress cron jobs to run at a system level with intervals of 15 minutes.

53. Failed Auto-Update
In order to help your site stay on the latest version of WordPress, you may have auto-updates enabled. This can be handy for streamlining this aspect of website maintenance and keeping your site secure, but it also sometimes results in problems.

Auto-updates can sometimes fail, in which case your site may go down and become unavailable to users. The recommended fix is to carry out a manual update instead.

100+ Most Common WordPress Errors and How to Fix Them

54. WordPress Import Issues
For a variety of reasons, you may find that you need to import content into your WordPress site. This is a fairly common practice among developers, and various plugins are often used for this task.

Unfortunately, imports can easily result in PHP or HTTP timeouts. In order to avoid these issues, you can:

Switch to a faster internet connection.
Import your files using the WP-CLI.
Increase your PHP timeout limit.
You may also need to contact your hosting provider for help resolving this issue.

55. WordPress Performance Issues
Your site’s performance is more or less synonymous with its speed. Fast-loading pages make for better UX and SEO, so it’s important to routinely monitor and optimize your site’s speed. Pingdom is a handy tool for testing loading times from multiple locations:

After testing your site, Pingdom will give you a list of suggestions regarding how you can improve its performance. Common solutions include image compression, caching, and enabling a CDN.

100+ Most Common WordPress Errors and How to Fix Them

56. WordPress Is Not Sending Emails
Email marketing is a key strategy for many WordPress sites and can increase your traffic level and conversion rates. There are several plugins available that can enable you to send emails from your WordPress dashboard, conveniently bundling your email marketing platform with your site’s backend.

Often, if your emails aren’t being sent to your subscribers, it’s because of your server’s configuration. Your host may have limits on the resources your site can use, which prevents emails from going out.

If you suspect a server-related issue, contact your host. You may need to upgrade your plan. Alternatively, the plugin you’re using could be the source of the problem. Check its support forums and documentation for common issues or contact the developer for support.

Finally, emails sent from WordPress may be marked as spam. If a user contacts you about a missing email, tell them to check their junk folder just in case.

100+ Most Common WordPress Errors and How to Fix Them

57. WordPress Syntax Errors
Syntax errors refer to problems with the syntax or structure of your code. This may include incorrectly-used punctuation marks or other typos. In some cases, a syntax error can lock you out of your dashboard and break your site.

Despite the seemingly-insignificant root cause, this type of error is pretty serious. It often occurs when you paste in code snippets you’ve found online. If you’ve done something like that recently, that’s likely the source of your problem.

To resolve it, navigate to the location of the code snippet you pasted in using FTP, and correct or remove it.

58. The WordPress Sidebar Is Appearing Below the Content
Sidebars can be useful for displaying key content to your users, such as your navigation menu, WordPress search function, social icons, and even disclaimers. If your sidebar looks odd because it’s appearing below your content instead of next to it, however, you’ve got a problem.

This is often the result of misused <div> tags in one or more of your theme’s files. You’ll need to track down the source of the issue in order to correct your code and fix it. This could also occur due to problems with your site’s width, afloat property error, or other issues with your WordPress theme.

59. White Text and Missing Buttons in the Visual Editor
Your WordPress editor is pretty important. Without it, adding new content to your site would be much more difficult. If you’ve ever opened the Classic Editor to find that all of the buttons are missing from the toolbar and your text color is set to white, you’ve probably felt the distress that comes with not having access to that functionality.

Often, this error is due to a plugin conflict or caching issue. If clearing your browser cache or deactivating your plugins doesn’t resolve the problem, you may need to replace some of your WordPress core files.

60. WordPress RSS Feed Issues
RSS feeds are an easy way to bolster your site through curation. They’re especially useful for news sites and other content hubs. However, errors in your RSS feed can appear unprofessional and prevent users from viewing content.

These errors may occur due to extra spaces or line breaks following closing PHP tags in your functions.php file or plugins. You can track them down and remove them to eliminate this issue. Alternatively, you may also need to test for plugin and theme incompatibilities or simply disable WordPress’ default RSS feeds function.

100+ Most Common WordPress Errors and How to Fix Them

61. WordPress Failed to Open Stream
If you see an error message reading “failed to open stream”, this means that WordPress was unable to open a file referenced somewhere in your code.

This error can be caused by a variety of issues, but the message will usually tell you what the source of the problem is. Possible responses include:

No such file or directory.
Permission denied.
Operation failed.
The course of action needed to correct the problem will depend on which response you’re seeing. It may be that there’s a file missing, your permissions are set incorrectly, or WordPress is having trouble connecting to a third-party API.

62. Password Reset Key Error
If users are able to register for accounts on your site, they may at times need to reset their passwords. In some cases, the default password reset email provides a link that directs users back to the login page, where they’ll see a message that reads: “This key is invalid or has been used. Please try to reset the password again.”

Usually, this is a caching issue. If you have a caching plugin installed on your site, make sure you’ve disabled caching for the My Account page in the plugin’s settings. Instances of conflicts with CAPTCHA plugins have also been reported.

100+ Most Common WordPress Errors and How to Fix Them

63. The Login Page Keeps Refreshing
If clicking on the login button on your WordPress login page simply refreshes it instead of bringing you to your dashboard, there may be something wrong going on:


100+ Most Common WordPress Errors and How to Fix Them
This issue may be due to a plugin conflict, wrong WordPress addresses, or a corrupted .htaccess file.

64. WordPress Keeps Logging You Out
Unlike the login page refreshing error, this problem enables you to briefly access your WordPress dashboard but then suddenly logs you back out. This is often due to an issue with your WordPress site’s settings.

If you’re experiencing this error, the WordPress Address and Site Address in your General settings probably don’t match:

This can include seemingly small differences, such as whether or not both URLs include www at the beginning. Changing the URLs so they match should fix this issue.

If you aren’t able to do this via your dashboard because WordPress keeps logging you out, you can get the job done by editing your wp-config.php file.

100+ Most Common WordPress Errors and How to Fix Them

65. “Are You Sure You Want to Do This?”
The most frustrating WordPress errors are those that give no indication as to what might be causing them. An error reading “Are you sure you want to do this?” is one such issue.

Most often, this is the result of a plugin or theme conflict and can be resolved with standard troubleshooting for that situation. In the event that this doesn’t work, you will probably need to replace your wp-config.php file.

66. “Another Update In Progress”
Normally, the “Another update is currently in progress” error appears if you’re trying to run a plugin or theme update while WordPress is still executing a core update.

Often this happens during automated core security updates. The message should automatically disappear once the first update has finished. If it doesn’t, you have an error on your hands. You can resolve it in phpMyAdmin by deleting the core_updater.lock row from the wp_options table.

67. Error Moving to Trash
WordPress enables you to easily delete posts and pages from your site with the click of a button. However, various problems can lead to an error when trying to move content to the trash.

This can occur because of a caching issue or a plugin conflict. It may also be due to database corruption or incorrect file permissions.

68. WordPress Installation Errors
Although WordPress is famous for its simple five-minute installation process, you may still run into trouble. Potential issues include the Error Establishing a Database Connection and 500 Internal Server Errors, which we’ve covered elsewhere in this post.

You may also encounter a “Headers Already Sent” error message. This is likely due to unnecessary spaces or PHP tags in your code. The message should tell you where the problem is and you can resolve it by editing the relevant file.

100+ Most Common WordPress Errors and How to Fix Them

69. “The Site Is Experiencing Technical Difficulties”
This error has become more frequent since the launch of WordPress 5.2. It usually appears during core, plugin, or theme updates:

An error message reading: “The site is experiencing technical difficulties.”

The cause of the “The Site Is Experiencing Technical Difficulties” error is typically either a PHP memory limit error or a plugin conflict. You can increase your site’s memory in different ways.

To troubleshoot a plugin conflict, try deactivating your plugins and then reactivating them one by one to see which one causes the error to appear again.

Info
The default memory limit for Kinsta customers is set to 256 MB. If you host your WordPress site at Kinsta you shouldn’t have any issues with a lack of memory.

70. “An automated WordPress update has failed to complete – please attempt the update again now”
You may have come across this error at the top of your WordPress admin dashboard: “An automated WordPress update has failed to complete – please attempt the update again now.”

This error is often caused by WordPress going into ‘maintenance mode’ after updates have been made to themes, plugins, or WordPress itself.

This error can usually be resolved by manually updating any failed automated updates.

If the message persists, it may be due to your WordPress site being stuck in ‘maintenance mode. This can be fixed by removing the “.maintenance” file from the root folder of your WordPress site, either via cPanel or using SFTP. Check out our guide to fixing WordPress Stuck in Maintenance Mode for step-by-step instructions.

71. Your WordPress Site Is Down
An unavailable site can lead to lost traffic and revenue. If you’re sure that your WordPress site is down, the first step is determining if the cause is a WordPress error or if your server is experiencing trouble. Symptoms of other WordPress errors may tip you off to the underlying problem.

If none are present, you can try checking your server’s error logs.

If your server is unable to work properly or has no idea about what’s happening, you should contact your hosting provider for help. Steps to fixing any #WordPress error:

100+ Most Common WordPress Errors and How to Fix Them

Summary
The last thing any site owner wants is for their WordPress website to become unavailable to users or to show issues. Not only does this cause you to miss out on any sales, ad views, SEO, conversions, and even affiliate commissions you might have earned.

It’ll also make your site seem less reliable and hurt your brand reputation, which could be really hard to repair.

That’s why we grouped these common WordPress errors all together on a single page to help you find a fix as easily as possible and get your business back on track quickly. Isn’t that convenient?

Do you have any questions about troubleshooting errors on your WordPress site? Ask away in the comments section below!

Save time, and costs and maximize site performance with:

Instant help from WordPress hosting experts, 24/7.
Cloudflare Enterprise integration.
The global audience reaches 33 data centers worldwide.
Optimization with our built-in Application Performance Monitoring.
All of that and much more, in one plan with no long-term contracts, assisted migrations, and a 30-day-money-back-guarantee. Check out our plans or talk to sales to find the plan that’s right for you.

100+ Most Common WordPress Errors and How to Fix Them

More 15 Most Common WordPress Errors and How to Fix Them
Web users are used to being presented with an HTTP error message, usually when a page they were attempting to access fails to load correctly. To determine why you received an error message and how to fix the issue, you need to understand what the various error codes mean. We have compiled the Top 15 Most Common Website Errors: what they mean, what causes them, and how to fix them.

Top 15 Most Common Website Errors: what they mean, what causes them, and how to fix them.
500 Internal Server Error
401 Unauthorised
400 Bad Request
403 Forbidden
404 Not Found
501 Not Implemented
502 Service Temporarily Overloaded
503 Service Unavailable
Connection Refused by Host
File Contains No Data
Cannot Add Form Submission Result to Bookmark List
Helper Application Not Found
TCP Error Encountered While Sending Request to Server
Failed DNS Look-Up
408 – Request Time-Out
100+ Most Common WordPress Errors and How to Fix Them
1. 500 Internal Server Error
This is hands down the most common error message web users will experience. This is a general-purpose error and can occur whenever an internal problem is encountered by a web server. More often than not, Error 500 occurs when the webserver is overloaded.

When you encounter this error message you can try to resolve it by reloading the page, clearing your browser’s cache, deleting your browser’s cookies, and restarting the browser. If you find this error occurring on your website, you should contact your hosting provider and, if you are running a WordPress site, test one by one any third-party plug-ins you may be using. 

2. 401 Unauthorised: 
This error message will appear usually after a user has attempted to access a site they were unauthorized to access or after a failed login attempt. As a website owner, you are able to add password protection to your site via your cPanel account. This can be a great extra security layer that restricts access to your admin area, such as the wp-admin folder in a WordPress site. 

3. 400 Bad Request: 
If your request is corrupted you will see this error message appear. It means that something has gone wrong with your web browser in relation to your request. Usually, this means the data sent by the browser does not conform to the rules of the HTTP protocol. The server does not know how to process a request with a malformed syntax. This can mean there is something unstable on the user’s side (unstable internet connection, a security issue within the operating system, a caching problem, or a defective browser). 

4. 403 Forbidden: 
If there is an attempt to access a forbidden directory on a website you will see this error message which means there is no login opportunity on the page. The most common reason a user will see this error message is if the website does not permit users to browse the site’s file directory structure or the specific file requested is not permitted to be viewed from the web.

You are able to set 403 protection on your own site for security reasons – hiding the directory structure or files that contain vulnerable information is a good way to harden your site against being hacked. Although many web hosts will offer this service to their clients by default, to add an extra security layer to your site simply open your cPanel account, navigate to the Advanced menu box and select Index Manager. From here you are able to customize how your users will view a specific directory on your website by selecting ‘No Indexing’ on the directory you wish to protect. 

100+ Most Common WordPress Errors and How to Fix Them

5. 404 Not Found: 
If a user attempts to access a non-existent web page, a 404 Not Found error message will appear. This message usually appears when a user closes the browser, hits the stop button or clicks on a link too quickly – however, this message may also appear when a file is very large or if a server is running too slow. 

The 404 error is likely to be one you have come across yourself while web-browsing. If the server cannot find anything on the requested location you will see a 404 message. Often this is simply due to a mistyped URL, but can also appear when users are attempting to access removed pages or pages that are temporarily unavailable. You want to reduce the number of 404s on your website wherever possible because they will most certainly increase your bounce rate. 

It should be noted that the 404 message is very close to the 410 – Gone error page. While both mean that the server could not find the requested file, the 410 indicates that this is a permanent situation, meaning the resource was likely intentionally made unavailable. To enhance your Google-friendliness, it is worthwhile knowing the difference between the two. You can learn more now by watching the video Does Google treat 404 and 410 status codes differently? 

100+ Most Common WordPress Errors and How to Fix Them
6. 501 Not Implemented: 
This message means that the browser does not support the requested feature. 

7. 502 Service Temporarily Overloaded: 
You will see a 502 error when your server is congested – a problem that usually resolves itself when web traffic decreases. 

8. 503 Service Unavailable: 
Users will see a 503 message if the site they are attempting to reach is busy, or if the server is down.

9. Connection Refused by Host: 
This error message, like the 403 error, usually means that the user does not have the authorization to access the site or that an attempted login failed, usually because the password used was not correct.

10. File Contains No Data: 
Users will see a File Contains No Data error when a page is present, but nothing shows up. This can be caused by bad table formatting or stripped header information. 

11. Cannot Add Form Submission Result to Bookmark List: 
When a user attempts to save a type of form that is not a document or a web address they will get this error.

100+ Most Common WordPress Errors and How to Fix Them

12. Helper Application Not Found: 
When a server cannot find the helper application required to download a file, this error may appear. 

13. TCP Error Encountered While Sending Request to Server: 
When there is a problem on the line between the user and the requested site, this error message will appear. As this can often be a hardware-related issue, this error should always be reported to a network administrator. 

14. Failed DNS Look-Up: 
When a website’s URL cannot be translated, a Failed DNS Look-Up error usually appears. This error usually appears on commercial sites due to overload. 

15. 408 – Request Time-Out: 
You will see this error message when the server does not receive the full request from the user within the set timeframe it has allocated to wait. Repeated 408s will occur if either the server or the user’s system is experiencing a heavy workload, or if there is a temporary internet surge that slows down the message being delivered to the server. The best immediate step you can take when you get a 408 error message is to reload the page and see if the issue persists. 

100+ Most Common WordPress Errors and How to Fix Them
Cheat Sheet
An easy way to determine what any status code means can be found with the number they begin with. The status code will usually be a three-digit number, therefore examples of a 5xx code would include error messages 501, 502, 503, etc. 

A little cheat sheet to help you narrow down what the issue is as follows: 

1xx codes:       Informational statuses.

2xx codes:       Statuses after a successful action.

3xx codes:       Statuses showing a redirection.

4xx codes:       Statuses showing a client-side error.

5xx codes:       Statuses showing a server-side error. 


