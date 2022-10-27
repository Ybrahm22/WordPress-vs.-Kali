# WordPress-vs.-Kali
# Project 7 - WordPress Pen Testing

Time spent: **12** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pen Testing Report

### 1. XSS Media Upload

- [ ] Summary: 
  - Vulnerability types: XSS 
  - Tested in version: 4.7
  - Fixed in version: 4.7.3
- [ ] GIF Walkthrough: <img src='https://github.com/Ybrahm22/WordPress-vs.-Kali/blob/main/XSS%204.7.gif' title='Media XSS Upload Exploit' width='' alt='Media XSS Upload Exploit' />
- [ ] Steps to recreate: 1. Get an upload compatible image from google. 2. Change image name to the JS XSS exploit. 3. Upload media 4. View post to trigger alert. 

  
### 2. XSS Hover over link

- [ ] Summary: 
  - Vulnerability types: XSS
  - Tested in version: 5.3
  - Fixed in version: 5.3.1
- [ ] GIF Walkthrough: <img src='https://github.com/Ybrahm22/WordPress-vs.-Kali/blob/main/Authenticated%20Stored%20Cross-Site%20Scripting%20(XSS)%205.3.gif' title='Stored Hover Over Link XSS' width='' alt='Stored Hover Over Link XSS' />
- [ ] Steps to recreate: 1. Authenticated user creates a post. 2. Add XSS code in the post. 3. View post. 4. Anytime user hovers their mouse over the link, XSS is triggered

### 3. XSS Onload Youtube Link

- [ ] Summary: 
  - Vulnerability types: XSS
  - Tested in version: 4.6
  - Fixed in version: 4.7.2
- [ ] GIF Walkthrough: <img src='https://github.com/Ybrahm22/WordPress-vs.-Kali/blob/main/Onload%20XSS%204.6.gif' title='XSS Onload Youtube Link
' width='' alt='XSS Onload Youtube Link' />
- [ ] Steps to recreate: 1. Authenticated user creates a post. 2. In textfield add the onload XSS code. 3. After publish, whenever the post is accessed or refreshed the XSS will trigger. 


## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with LICECAP ...
<!-- LiceCap -->

## Notes

Had lots of trouble with degrading Wordpress version due to internal changes. Numerous issues with Wordpress container on Docker. 

## License

    Copyright [2022] [Yug Brahmbhatt]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
