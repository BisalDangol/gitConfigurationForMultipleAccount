# Git Configuration For Multiple Account
**Git Configuration For Multiple Account using Https method.** 
Managing multiple Git accounts on a single machine can be done by configuring Git to distinguish between accounts using different SSH keys or HTTPS credentials. There are two main ways to handle this in Git Bash. This guide will walk you through the steps to manage multiple accounts.

Using HTTPS for multiple Git accounts is a simpler and more secure way to authenticate with repositories, especially in situations where SSH may not be as convenient. For example, when working on machines without SSH key support or in environments with strict network restrictions, HTTPS provides an effective solution.

## Managing Multiple Accounts with HTTPS:
When using multiple Git accounts via HTTPS, you can still configure Git to handle different credentials for different repositories. Unlike SSH keys, which require configuring SSH agent and key files, HTTPS authentication typically relies on username and password or personal access tokens (PATs) for secure login. Followig steps can help to setup the multiple account in git bash.

**Steps 1: Open git bash if you are using windows otherwise OS's terminal can work perfectly**

**Steps 2: Open your github page and navigate through it.**

<img src="https://github.com/BisalDangol/gitConfigurationForMultipleAccount/blob/main/Seting%20in%20Github.png">

**Steps 3: Click on Developer Setting**

<img src="https://github.com/BisalDangol/gitConfigurationForMultipleAccount/blob/main/Developer%20Option.png">

**Steps 4: click on Personal Access token. You can view more option click on Tokens**

<img src="https://github.com/BisalDangol/gitConfigurationForMultipleAccount/blob/main/Personal%20Access%20Tokens%20(PAT).png">
<img src="https://github.com/BisalDangol/gitConfigurationForMultipleAccount/blob/main/tokenInGit.png">


**Steps :**
**Steps :**
**Steps :**


**Steps 2:**
   ```bash
   git config --global user.name
  ```

http://github.com/BisalDangol/gitConfigurationForMultipleAccount/blob/main/tokenInGit.png
## Advantages of Using HTTPS:
1. Ease of Setup: HTTPS is easier to set up than SSH, especially for new users or environments that don’t support SSH keys (e.g., corporate environments or shared servers). You only need to enter your username and password (or PAT) for authentication.
2. No Need for SSH Keys: HTTPS avoids the need to generate and manage SSH keys. This is especially useful if you're working on a machine where SSH key configuration is difficult or impractical.
3. Cross-Platform Compatibility: HTTPS is universally supported and works on any platform without the need for additional configurations like SSH agents or key files. It works in environments where SSH might be restricted (e.g., firewalls blocking SSH traffic).
4. Security with Tokens: Personal Access Tokens are more secure than passwords and provide fine-grained control over access. You can create tokens with specific permissions and expiration dates, enhancing security compared to traditional password-based authentication.
5. Simpler Authentication: Using HTTPS is typically simpler than SSH for users who are unfamiliar with key management. Most Git hosting services provide intuitive instructions for setting up HTTPS authentication, making it easy for new users to get started.

## Disadvantage of Using Https:
- Frequent Credential Entry: Without credential caching, you may need to enter your username and password (or token) every time you interact with the repository.

# Conclusion:
Using HTTPS to manage multiple Git accounts is a good choice when we prioritize simplicity and compatibility across platforms. By caching credentials or using a credential manager, we can minimize the need to manually enter credentials, making it almost as convenient as SSH, but without the need for managing SSH keys.
#
