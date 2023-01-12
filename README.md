# Welcome to Burmis Studios!

Within this readme is some tips and set up required to be productive with Burmis. This includes tooling, account setup, and code-base standards. This guide will not include absolutely everything! Please refer any extra or unclear questions to [Mark](mailto:mark@burmis.ca) or an appropriate team member!

---

## Contents

- [Welcome to Burmis Studios!](#welcome-to-burmis-studios)
  - [Contents](#contents)
  - [Accounts](#accounts)
    - [Github 2FA / Commit Signing](#github-2fa--commit-signing)
    - [Gmail/Gchat/Gmeet](#gmailgchatgmeet)
    - [1Password](#1password)
    - [Toggl](#toggl)
  - [Extras](#extras)
    - [Github Notifier](#github-notifier)
    - [Github Mobile](#github-mobile)
  - [Payment Information](#payment-information)
    - [GST Number](#gst-number)
    - [Billing](#billing)
  - [Code Standards](#code-standards)
    - [End of File](#end-of-file)
    - [End of Line](#end-of-line)
    - [Don't Play Code Golf](#dont-play-code-golf)
    - [Prettier/Code Linting](#prettiercode-linting)
    - [Workflow](#workflow)
    - [Tests](#tests)
    - [Issues](#issues)
    - [Branching](#branching)
    - [Pull Requests](#pull-requests)
    - [Project Board](#project-board)

---

## Accounts

Burmis studios uses software solutions for most business tracking and access. Below is some information to help you get aquintated.

### Github 2FA / Commit Signing

> Burmis Studios required two-factor authentication on our developer's Github account as well as commit signing via GPG key. This is for extra security in our organizations repositories. 2FA should be set up regardless of Burmis, as it is in your best interest to protect your Github account. GPG signing keys help us keep the repo's secure by authenticating that commits actually came from who they should. If someone did get access to your account, it would be very difficult for them to commit malicious code to our code base.  

2FA is a quick and easy process that I'm sure most are familiar with already. Below are some documents for setting it up with your Github account.

- [Two-Factor Authentication](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)
 
As GPG keys are a fairly involved process to set up, I will again refer to Githubs official documentation. You can configure git on your computer to automatically request a signing / password input so that you never forget. Below are some links to documentation that should help you get this set up!

- [Commit Verification / Key Set-up](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification)
- [Using Key Automatically](https://docs.github.com/en/authentication/managing-commit-signature-verification/telling-git-about-your-signing-key)

### Gmail/Gchat/Gmeet
---
> Used for general communication purposes. This can all be handled with any email address, but gmail is preferred since most team members use it. We use Google Meet for video meetings, Google Chat for general day to day text chat, Google Calendar for scheduling, and Gmail for... Email!
>
> Google chat also has a nice teams feature, which is similar to Slack. You will be invited to these accordingly after your account is set up. 
>
> Please use a business appropriate email address! 

Since it is not totally obvious within Gmail, this is a convienent way to set up Google Chat.

![image](https://user-images.githubusercontent.com/48274410/208812226-7d8826da-0bbc-4977-a4c0-68a504e7550e.png)

- Click the "Settings" cog within the Gmail inbox. 
- Select "Apps in Gmail."
- Show "Chat and Meet in Gmail."

![image](https://user-images.githubusercontent.com/48274410/208812293-eedf8470-923f-4a33-a3ba-1fa0fa2e2ae4.png)

It should look like this afterwards. Now all company communication is in one convienent place! 

### 1Password 

> Used for access to different company software and development information, for example, TailWindUI accounts, ENV variables, and testing accounts for Swype.
>
> [Mark](mailto:mark@burmis.ca) will need to give you access to this, but you can go ahead and load it into your browser now. 

Please translate according to your own browser! These instructions will likely be similar.

- Navigate to the browser "Add-ons" or "Extensions"
- Search for and install 1Password
- Set up account and await access from Mark.

![image](https://user-images.githubusercontent.com/48274410/208812387-c35374dd-6420-4640-8bd2-2415e08ad938.png)

More information about accounts and how it works can be found in the [docs!](https://support.1password.com/explore/get-started/)

Once 1Password has been set up and given access, you will be able to see the different accounts available for development purposes. 

---

NOTE: Please only use these accounts for activities related to Burmis Studios.

---

### Toggl 

> Toggl is a convientent way to track your time against company projects for invoicing later. This will also require granted access from [Mark](mailto:mark@burmis.ca). 

Once again, please translate according to your own browser! These instructions will likely be similar.

- Navigate to the browser "Add-ons" or "Extensions"
- Search for and install Toggl Track
- Set up account, preferably the Gmail account you used or set up earlier

![image](https://user-images.githubusercontent.com/48274410/208812464-dc3a7bc3-a7a0-4cf5-a1a7-748b3331a4e8.png)

More information about accounts and how it works can be found on their [website!](https://toggl.com/?cq_src=google_ads&cq_cmp=15031885853&cq_term=&cq_plac=&cq_net=x&cq_plt=gp&utm_term=&utm_campaign=%5BPM%5D+-+Region+1+-+Generic+-+Billable+Events+-+Time+Tracking+Done+Right&utm_source=adwords&utm_medium=ppc&hsa_acc=8476800569&hsa_cam=15031885853&hsa_grp=&hsa_ad=&hsa_src=x&hsa_tgt=&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3&gclid=Cj0KCQiA14WdBhD8ARIsANao07gwUIRvIfdcGgNzID8ZSzGTudSGT0QBxZRNwTJ--FPH94CsrhG8TyEaArQ1EALw_wcB)

Once your account has been set up, you can begin tracking invoicable time as follows. 

- Near your address bar, you should see a Toggl add on button. 
- Fill in the "What are you working on?" text field with relevant information (ie. Description of what you are coding)
  - Please make sure to be at least a little descriptive! This will make invoicing easier later. 
- Click the play button
- Click on the description that you wrote earlier, which will now be displayed where the text box once was. This will reveal more options
- You can now choose which project your task is related too
- Select whether the time is billable or not (Most likely is)
- Click Done!

It is very important to not miss any description of tasks. If you do not have an explanation of why you logged hours, we have no way of telling the client why we are billing that time.

Make sure you describe your time entries accurately!

![image](https://user-images.githubusercontent.com/48274410/208812512-af8ddea0-7567-4f36-aa65-50f3a178da72.png)

Your time is now being tracked by the second (Just time, its not as sinister as it sounds). 

--- 

NOTE: Mistakes happen. Sometimes we get up from our PC, forget to pause our time and now we have logged a 21 hour nap. Do not worry! We can adjust this. 

- Open the add-on menu from the previous step. 
- Click on the Square & Arrow button to open the Toggl interface
- You can now drag, add, delete, adjust, and move time around by clicking on logged time slots like the Greek God Chronos

This interface is also what you will want to use for invoicing purposes. It will display all of your tracked time in a calendar, which can easily be translated to a formal invoice for billing, as described below. 

![image](https://user-images.githubusercontent.com/48274410/208812562-395428ab-3013-45c1-8aaa-8e24d060eb13.png)

---

## Extras

Here are some extra little things we use around the office to keep our workflow smooth!

### Github Notifier

> Github Notifier is another handy little browser extension that helps you keep on top of Github Notifications.

Never miss a change request again! Never miss a review request! This add-on will allow your browser to notify you of Github notifications convienently. Once again, make sure to adjust steps to match your browser. 

- Navigate to the browser "Add-ons" or "Extensions"
- Search for and install Github Notifier

![image](https://user-images.githubusercontent.com/48274410/209077061-33aa077b-4b2b-4944-b620-eda4a06e9ece.png)

Something to consider is that the set up for this add-on is a little more extensive. You will need to create a Github token with notification privelages for public repo's, or a token with repo AND notification for private repositories. This is a fairly involved process but there is plenty of documentation online that I will link to below. Whether it be for this add-on or not, you should get familiar with tokens! They are very useful to know. 

- [Creating a token](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

Here is a screen shot of the add-on initial configuration panel.

![image](https://user-images.githubusercontent.com/48274410/209076818-25c22ad8-d5da-41a5-9d33-b214a0753a1d.png)

NOTE: The Root URL for burmis is https://api.github.com/burmis

---

### Github Mobile

> Github provides a handy little application for mobile devices. This allows you to recieve notifications while on the run! 

- [Android Devices](https://play.google.com/store/apps/details?id=com.github.android)
- [Apple Devices](https://apps.apple.com/us/app/github/id1477376905)

Don't worry, there is dark mode. 

![image](https://user-images.githubusercontent.com/48274410/209076882-80f718a2-1c3a-4cf4-a284-502560baba0b.png)

---

## Payment Information

Below is some information regarding financials. 

### GST Number

> Since we are payed as contractors, you are REQUIRED to have a Canada GST number for invoicing. Thankfully, this is a very quick phone call and believe it or not, a relatively painless process. 

- Follow these [steps](https://www.canada.ca/en/revenue-agency/services/tax/businesses/topics/gst-hst-businesses/account-register.html)
- WRITE THIS NUMBER DOWN. You will need to record it on invoices.

---

### Billing 

> Billing is done by sending an invoice to [Mark](mailto:mark@burmis.ca). This step isn't standardized but make sure you use something professional. Personally, I just found a nice template from Google docs.

- Use the Toggl Interface as described [here](#toggl) to view your tracked time 
- Your invoice should look something similar to this...
- You NEED to have your...
  - [GST Number](#gst-number) IMPORTANT
  - Contact Information
    - Address
    - Phone Number
    - Email Address
  - Totaled up hours
  - Payment details (ie. Where do you want your money sent?)
- Below is a general example...

![image](https://user-images.githubusercontent.com/48274410/208813192-97825471-8265-4940-a19a-565e25a714cb.png)

- Send your invoice to [Mark](mailto:mark@burmis.ca)

--- 

NOTE: Please discuss your pay schedule preference with... you guess it, [Mark](mailto:mark@burmis.ca). He's a nice guy don't be shy. Also, payment is typically handled via eTransfer, hence the importance on payment details being on your invoice.  

---

## Code Standards 

Below are some house standards regarding code. 

### End of File

> Please always include one empty line at the end of each file. It makes ```git diff``` much easier to read, and lines up changes on Pull Requests.

EXAMPLE:

```js
const ExampleFunction = () => {
    ...
};

export default ExampleFunction;
// NEW LINE
```

---

### End of Line

> Most of our developers use Linux. As such, line endings have caused problems between devs due to Windows using ```CRLF``` and Linux using ```LF```. Please default your editor to ```LF``` as it is cross compatible and will save a myriad of linting headaches. 

If you are using Visual Studio Code as most of us do...

- Bottom right of VSCode...

![image](https://user-images.githubusercontent.com/48274410/208813328-6efce83f-1d53-4e20-92cd-2695d3b7641f.png)

![image](https://user-images.githubusercontent.com/48274410/208813359-342d2bb2-ef32-4848-af7b-9ffb0bca396d.png)

OR 

- CNTRL + SHIFT + P

![image](https://user-images.githubusercontent.com/48274410/208813607-311e9b9a-cf32-49cb-95ac-4b4236519630.png)

![image](https://user-images.githubusercontent.com/48274410/208813359-342d2bb2-ef32-4848-af7b-9ffb0bca396d.png)

### Don't Play Code Golf

> We have multiple developers working on the same project at times. While it may be impressive to reduce a 50 line function to a heiroglypic one liner, it is usually not fun for the next dev who may have to decipher it. Please save it for Leetcode! (and send it around so we can marvel at it)

Read this and cry! [Code Golf](https://dev.to/emnudge/js-code-golfing-how-to-ruin-everyone-s-day-40h3)

---

### Prettier/Code Linting

> Most of our projects include some sort of built in project linter or formatting tool. It is wise to run these commands before committing your code, as GitHub will get angry at you if you fail the [tests](#tests).
>
> Since this will be project specific, it is hard to write a clear example. Please ask a colleague for more information on your specific project! Most project > will have some sort of script to check for these problems, most commonly, ```yarn lint```.

---

### Workflow 

> A general overview of the Burmis workflow is below. There are a few moving parts with many sections of their own. While it may seem like a lot, it is a pretty standard workflow across many organizations. Click around to other sections for clarification! Keeping this process standardized helps things move smoothly. 

This is what a typical task looks like from beginning to end. 

- An [issue](#issues) in your repository has been created, and marked as TODO.
- You view it on the [project board](#project-board)  
- You are assigned that [issue](#issues) or decide you want to tackle it. 
- You make a [branch](#branching) off of ```main``` in your repo. 
- You write your code, fix the issue, make the adjustments
- You ensure this new code passes [lints](#prettiercode-linting) and [tests](#tests)
- Commit the new code to YOUR [branch](#branching), not ```main```
- You create a new draft [pull request](#pull-requests)
- Select a [reviewer](#reviews)
- Fill in [pull request](#pull-requests) information
- Mark [pull request](#pull-requests) as ready for [review](#reviews), and await
- If [pull request](#pull-requests) is approved without changes, [Squash and Merge!](#pull-requests)
- If [change requests](#pull-requests) are made, review changes, and adjust until approved or closed
- Adjust the [project board!](#project-board)

---

NOTE: Please ask questions to any team members for clarification at ANY point of the process! It is better to ask first and clarify, than it is to assume and make a mistake. (Not that we will hold it against you)

---

### Tests

> Many projects include handy little Github actions and testing scripts that automatically catch us from merging or committing broken code.

Usually a project will include a testing script that you can run to check for any blaring errors in your branch before committing it. This is a good habit to form as it will save some headaches during [pull requests](#pull-requests). For example, ```yarn test```. Make sure these test pass before committing your code!

Git hub actions will usually run on push, but othertimes as well. NO reviewer will approve a PR with failing tests, so make sure they are fixed before hand. Usually, your terminal will give you some feedback on why they are failling. Github Actions can also be explored here in a terminal style. 

### Issues

> Issues are a handy Github feature to keep track of what needs to be done or fixed on a repository.

![image](https://user-images.githubusercontent.com/48274410/208813869-fe128cc0-1d82-49c3-b330-c1d82f7b44a9.png)

Typically, an issue will include information about the task, a checklist of what needs to be completed, instructions on how to reproduce a bug, or just a general walk through of the task itself. This is usually where you can answer the age old question, "What can I do?" Issues are held within the the repository for viewing, or on the [project board](#project-board).

- If you decide to tackle a particular issue, please assign it to yourself! This helps the team track who is working on what. 

![image](https://user-images.githubusercontent.com/48274410/208813970-da50b79f-6ea8-40ad-afd3-5c75804e9a68.png)

- After you are assigned an issue, please view [branching](#branching)
---

### Branching

> Burmis studios has a few standards regarding creating a branch.

When you are assigned an issue, the [workflow](#workflow) requires a new branch. 

- Always branch off ```main``` in your related repository.
- Name your branch according to the issue. (ex. issueNumber-branch-name)

---

### Pull Requests

> Burmis never commits directly to main. All code changes are done through [branches](#branches) and [pull requests](#pull-requests).

Once your issue has been completed, its time to make a pull request! This can be a little intimidating at first, but gets easier with time. There a few steps you need to follow.

- Make sure all of your code passes [test](#tests) and [lints](#prettiercode-linting)
- Publish your [issue branch](#branching) to remote. (This may already be complete)
- The repo will have an indicator stating "There have been recent commits to ```issuenumber-issue-branch-name```. Compare and Pull Request?"
- The button attached to that indicator will create a new PR!

This is where the important specification follow, so please follow this process closely. 

- Create a Draft Pull Request immediately. This starts the Github action [testing](#tests) right away, and you won't have to wait 

![image](https://user-images.githubusercontent.com/48274410/208814216-f9917ba6-3eda-4472-b1c1-e45dde8dceb5.png)

- Edit the PR and fill out ALL of the relevant details. Thankfully, there is usually a template. Below is an example...

![image](https://user-images.githubusercontent.com/48274410/209076710-deeb1cac-f120-4b79-9fa2-c2a35e24951e.png)

  - NOTE: If you use ```Fixes #issueNumber``` in your PR description your issue will automatically close when your branch is merged.
- Select a reviewer

![image](https://user-images.githubusercontent.com/48274410/208814297-d8ad16d0-c392-41bc-a119-17e3116aa0d6.png)

  - All PR's require a reviewer. Try to rotate your reviewers so that everyone is familiar with multiple sections of the codebase

![image](https://user-images.githubusercontent.com/48274410/208814902-f9f1fc76-8fb4-4a82-9155-10e559dd0d6f.png)

- Await all [tests](#tests) to pass and make sure they succeed
- If it is all green and succeeded, mark PR as Ready for Review!

![image](https://user-images.githubusercontent.com/48274410/208814461-651377c4-7a09-4e80-869a-ba9b955f05b2.png)

- Update [project board](#project-board)

> Sometimes, we nail it on the first try. If your PR is approved, go ahead and merge your PR!

- Always use SQUASH AND MERGE. This keeps our commit history on ```main``` from getting out of control.

![image](https://user-images.githubusercontent.com/48274410/208814495-f3c1d63a-5dc3-4cc7-87db-bf9b8e4d03e6.png)

>Sometimes, we don't nail it on the first try, or the second, or the fiftieth, and thats okay. Some issues are hard. If you reviewer requests changes, you will have to review and make the changes, or discuss them with your reviewer. Essentially, you are reset to the top of the above list, except the pull request already exists. Any commits that you make to the issue branch will be recorded on the PR you already made. Make the changes, and rerequest a review when you are ready!

---

### Project Board

> Project board is a rather new feature to Github that Burmis uses to keep track of workflow on projects. 

Within the project board, you can find all of the same issues within the "[Issues](#issues)" section of a repository. The main difference however, is the nice click and drag interface that lets us categorize tasks into different phases of developement. The interface is very self explanitory. Clicking on an [Issue](#Issues) will show more details about it, and you are able to click and drag them into different sections accordingly. Please keep this board up to date as you complete and move through tasks!

Some categories include... 

- ```Proposed``` (Not quite ready to start, but in the works.) 
- ```TODO``` (Ready to go! We are clear and ready for a developer to begin working on this issue.)
- ```Blocked``` (The worst! We have some sort of currently insurpassable blockage that prevents work on this issue.)
- ```In Progress``` (Whoever is listed as "Assigned" is currently working on this issue. Beat you to it!)
- ```Ready for Review``` (This issue currently has an open [PR](#pull-requests) that is awaiting review! Maybe yours!)
- ```Done``` (This task has been completed. Hooray!) 

As you move through your task list or issue, please return to and update this board accordingly. It helps keep everyone on the same page!

---
