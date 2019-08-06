# Phone_Gap

Hello World PhoneGap Template bitHound Score
A PhoneGap Hello World template

Usage
PhoneGap CLI
The hello-world template is the default when you create a new application using the phonegap-cli.

phonegap create my-app
Create an app using this template specifically:

phonegap create my-app --template hello-world
To see a list of other available PhoneGap templates:

phonegap template list
config.xml
android-minSdkVersion (Android only)
Minimum SDK version supported on the target device. Maximum version is blank by default.

This template sets the minimum to 14.

<preference name="android-minSdkVersion" value="14" />
<access ...> (All)
This template defaults to wide open access.

<access origin="*" />
It is strongly encouraged that you restrict access to external resources in your application before releasing to production.

For more information on whitelist configuration, see the Cordova Whitelist Guide and the Cordova Whitelist Plugin documentation

www/index.html
Content Security Policy (CSP)
The default CSP is similarly open:

<meta http-equiv="Content-Security-Policy" content="default-src * 'unsafe-inline'; style-src 'self' 'unsafe-inline'; media-src *" />
Much like the access tag above, you are strongly encouraged to use a more restrictive CSP in production.

A good starting point declaration might be:

<meta http-equiv="Content-Security-Policy" content="default-src 'self' data: gap: 'unsafe-inline' https://ssl.gstatic.com; style-src 'self' 'unsafe-inline'; media-src *" />
For more information on the Content Security Policy, see the section on CSP in the Cordova Whitelist Plugin documentation.

Another good resource for generating a good CSP declaration is CSP is Awesome
