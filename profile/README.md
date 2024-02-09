# OnlyAuth: 2FA API for Developers and Enterprises Alike
Today the world of 2FA is divided into two main categories: OTP codes via SMS and the usage of Authenticator Apps.

And the reality of what MFA truly is, and what is being offered today is vastly different.


## What's wrong with 2FA SMS
Sending an OTP code via SMS is super easy to get started. Usually you start with just a few lines of code with your favorite telco API provider. You then push it to the internet, and you notice suddenly you are getting a high SMS bill. This is when you learn what SMS Pumping is. You learn how to fix it, and then you release a new version of your app.

Unfortunately your SMS bill just continues to rise despite the fixes for SMS Pumping. Now you have to learn the hard way what Toll Fraud is. So you learn again how to fix it, and release a new version.

This pattern is extremely common for many developers - and if your app is especially popular, you will begin to feel the pain of monthly SMS charges eating into your profit.

Meanwhile you are doing all of this, SMS is inherently insecure. And there is nothing you can do about it! There is no such thing as end-to-end encryption in the telephony world. SMS Hijacking continues to rise exponentially year-over-year.

So something you thought that was easy to build, you now have had to release multiple fixes, it's expensive _AND_ insecure.


## Authenticator Apps
TOTP, or the use of Authenticator Apps like Google Authenticator, Authy are a slightly different story. These are inherently secure so long as you implement it properly (recently there was a startup that leaked and exposed TOTP secrets and backup codes, so you still have to know what you are doing), but the main problem is it's difficult for end-users. If all of your users are technical, then it's less of a barrier, but if a percent of your users are non-technical, then you are going to have problems getting them onboard.


And you will run into the increase of customer service tickets; the people who replaced/lost their phones, didn't backup their recovery codes, and everything in between.


## So what is OnlyAuth?
OnlyAuth is founded by people who are tired of the status quo in 2FA. And so far we have just talked about Two-Factor Authentication, let alone MFA. 

We believe in a future where users can decide how much security they want to add to their accounts (hello back accounts - let me authenticate with my password, and then a touch of my Yubikey). There are better channels than just SMS and Authenticator apps as well - be it biometrics, FIDO security keys, push notifications, Passkeys and more.


OnlyAuth is an API that is built for developers to quickly add these 2FA channels, and allow their users to authenticate 2FA (or even MFA) in channels that work best for them. Meanwhile it's easy for developers to add, maintain, and scale two-factor authentication in their apps.

## What about MFA?
Today there are a significant number of companies that use 2FA and MFA interchangeably. This is just incorrect, and truly unfortunate for us users who truly want digital security.

MFA, or multi-factor authentication is simply more 2FA channels than just a secondary one (hence the word _multi_). So for an example you can login with a username and password, and then have TOTP, this is an example of 2FA. But if you then authenticate with a Yubikey, then this is true MFA, as you now have two factors apart from your password. 

We believe that for some users for some accounts, MFA is needed, or at least offered as a choice. Today, us as users, are rarely given that choice. 


## What is the 2FA/MFA API?
Today we are at version 0.01 in this journey. But check out our [API developer docs for the 2FA API](https://www.onlyauth.io/docs), and give us feedback you have (especially the negative bit). Being developers ourselves, we understand how important other devs' feedback is, and we truly do act on it.

#

We are still super early in this journey, but we want you to be a part of it. Leave a comment on one of our repos, check out our website at [https://www.onlyauth.io](https://www.onlyauth.io) or drop us an email at [hello@onlyauth.io](mailto:hello@onlyauth.io).


Let’s redefine what’s possible in digital security together.
