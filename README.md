# Codepath
# Project 7 - WordPress Pentesting

Time spent: 6 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Unauthenticated Stored Cross-Site Scripting(XSS)
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: 
     <img src="https://github.com/nayanika96/Codepath-/blob/master/xss1.gif" width="800">
  - [ ] Steps to recreate: 
     1. Log in to the admin site
     1. Post a comment on the wordpress site using a string of code given in the source code
     3. Edit the comment by replacing the end of the code with 64kb of random text 
  - [ ] Affected source code:
    - [Link 1](https://klikki.fi/adv/wordpress2.html))
    
1. (Required)  Authenticated Stored Cross-Site Scripting(XSS) in Youtube URL Embeds
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.7
  - [ ] GIF Walkthrough: 
  <img src="https://github.com/nayanika96/Codepath-/blob/master/youtubeerror.gif" width="800">
  
  - [ ] Steps to recreate: 
     1. Log in on the admin wordpress site
     2. Create a new post with a youtube link
     3. Replace the end of the URL with <script>alert('XSS!');</script>
       
  - [ ] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca)
    
1. (Required)  Authenticated Stored Cross-Site Scripting
  - [ ] Summary: 
    - Vulnerability types:XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: 
    <img src="https://github.com/nayanika96/Codepath-/blob/master/scriptlink.gif" width="800">
  - [ ] Steps to recreate: 
     1. Log into admin account on wordpress
     2. Create a post
     3. Add code to the post as shown in the source code After submitting the costp, an alert box shows up which can be further modified by an attacker with a malicious attack.  
  - [ ] Affected source code:
    - [Link 1](https://klikki.fi/adv/wordpress3.html))


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
