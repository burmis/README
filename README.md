# Welcome to Burmis Studios!

Within this readme is some tips and set up required to be productive with Burmis. This includes tooling, account setup, and code-base standards. Please refer any extra or unclear questions to [Mark Bennett](mailto:mark@burmis.ca)!

---

## Accounts

Burmis studios uses software solutions for most business tracking and access. Below is some information to help you get aquintated.  

### Gmail/Gchat/Gmeet
---
> Used for general communication purposes. This can all be handled with any email address, but gmail is preferred since most team members use it. We use Google Meet for video meetings, Google Chat for general day to day text chat, Google Calendar for scheduling, and Gmail for... Email!
>
> Google chat also has a nice teams feature, which is similar to Slack. You will be invited to these accordingly after your account is set up. 
>
> Please use a business appropriate email address! 

Since it is not totally obvious within Gmail, this is a convienent way to set up Google Chat.

- Click the "Settings" cog within the Gmail inbox. 
- Select "Apps in Gmail."
- Show "Chat and Meet in Gmail."

Now all company communication is in one convienent place! 

### 1Password 

> Used for access to different company software and development information, for example, TailWindUI accounts, ENV variables, and testing accounts for Swype.
>
> [Mark Bennett](mailto:mark@burmis.ca) will need to give you access to this, but you can go ahead and load it into your browser now. 

Please translate according to your own browser! These instructions will likely be similar.

- Navigate to the browser "Add-ons" or "Extensions"
- Search for and install 1Password
- Set up account and await access from Mark. 

More information about accounts and how it works can be found in the [docs!](https://support.1password.com/explore/get-started/)

Once 1Password has been set up and given access, you will be able to see the different accounts available for development purposes. 

---

NOTE: Please only use these accounts for activities related to Burmis Studios.

---

### Toggl 

> Toggl is a convientent way to track your time against company projects for invoicing later. This will also require granted access from [Mark Bennett](mailto:mark@burmis.ca). 

Once again, please translate according to your own browser! These instructions will likely be similar.

- Navigate to the browser "Add-ons" or "Extensions"
- Search for and install Toggl Track
- Set up account, preferably the Gmail account you used or set up earlier

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

Your time is now being tracked by the second (Just time, its not as sinister as it sounds). 

--- 

NOTE: Mistakes happen. Sometimes we get up from our PC, forget to pause our time and now we have logged a 21 hour nap. Do not worry! We can adjust this. 

- Open the add-on menu from the previous step. 
- Click on the Square & Arrow button to open the Toggl interface
- You can now drag, add, delete, adjust, and move time around by clicking on logged time slots like the Greek God Chronos

This interface is also what you will want to use for invoicing purposes. It will display all of your tracked time in a calendar, which can easily be translated to a formal invoice for billing, as described below. 

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

- Use the Toggl Interface as described [here](###Toggl) to view your tracked time 
- Your invoice should look something similar to this...
- You NEED to have your...
  - [GST Number](###GSTNumber) IMPORTANT
  - Contact Information
    - Address
    - Phone Number
    - Email Address
  - Totaled up hours
  - Payment details (ie. Where do you want your money sent?)
- Below is a general example...
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

- Steps here. 

### Don't Play Code Golf

> We have multiple developers working on the same project at times. While it may be impressive to reduce a 50 line function to a heiroglypic one liner, it is usually not fun for the next dev who may have to decipher it. Please save it for Leetcode! (and send it around so we can marvel at it)

---

### Prettier/Code Linting

> Most of our projects include some sort of built in project linter or formatting tool. It is wise to run these commands before committing your code, as GitHub will get angry at you if you fail the [tests](###Tests).
>
> Since this will be project specific, it is hard to write a clear example. Please ask a colleague for more information on your specific project! Most project > will have some sort of script to check for these problems, most commonly, ```yarn lint```.

---

### Workflow 

> A general overview of the Burmis workflow is below. There are a few moving parts with many sections of their own. While it may seem like a lot, it is a pretty standard workflow across many organizations. Click around to other sections for clarification! Keeping this process standardized helps things move smoothly. 

This is what a typical task looks like from beginning to end. 

- An [issue](###Issues) in your repository has been created, and marked as TODO.
- You view it on the [project board](###ProjectBoard)  
- You are assigned that [issue](###Issues) or decide you want to tackle it. 
- You make a [branch](###Branching) off of ```main``` in your repo. 
- You write your code, fix the issue, make the adjustments
- You ensure this new code passes [lints](###Prettier/CodeLinting) and [tests](###Tests)
- Commit the new code to YOUR [branch](###Branching), not ```main```
- You create a new draft [pull request](###PullRequests)
- Select a [reviewer](###Reviews)
- Fill in [pull request](###PullRequests) information
- Mark [pull request](###PullRequests) as ready for [review](###Reviews), and await
- If [pull request](###PullRequests) is approved without changes, [Squash and Merge!](###PullRequests)
- If [change requests](###PullRequests) are made, review changes, and adjust until approved or closed
- Adjust the [project board!](###ProjectBoard)

---

NOTE: Please ask questions to any team members for clarification at ANY point of the process! It is better to ask first and clarify, than it is to assume and make a mistake. (Not that we will hold it against you)

---

### Tests

> Many projects include handy little Github actions and testing scripts that automatically catch us from merging or committing broken code.

Usually a project will include a testing script that you can run to check for any blaring errors in your branch before committing it. This is a good habit to form as it will save some headaches during [pull requests](###PullRequests). For example, ```yarn test```. Make sure these test pass before committing your code!

Git hub actions will usually run on push, but othertimes as well. NO reviewer will approve a PR with failing tests, so make sure they are fixed before hand. Usually, your terminal will give you some feedback on why they are failling. Github Actions can also be explored here in a terminal style. 

### Issues

> Issues are a handy Github feature to keep track of what needs to be done or fixed on a repository.

Typically, an issue will include information about the task, a checklist of what needs to be completed, instructions on how to reproduce a bug, or just a general walk through of the task itself. This is usually where you can answer the age old question, "What can I do?" Issues are held within the the repository for viewing, or on the [project board](###ProjectBoard).

- If you decide to tackle a particular issue, please assign it to yourself! This helps the team track who is working on what. 
- After you are assigned an issue, please view [branching](###Branching)
---

### Branching

> Burmis studios has a few standards regarding creating a branch.

When you are assigned an issue, the [workflow](###Workflow) requires a new branch. 

- Always branch off ```main``` in your related repository.
- Name your branch according to the issue. (ex. issueNumber-branch-name)

---

### Pull Requests

> Burmis never commits directly to main. All code changes are done through [branches](###Branches) and [pull requests](###PullRequests).

Once your issue has been completed, its time to make a pull request! This can be a little intimidating at first, but gets easier with time. There a few steps you need to follow.

- Make sure all of your code passes [test](###Tests) and [lints](###Prettier/CodeLinting)
- Publish your [issue branch](###Branching) to remote. (This may already be complete)
- The repo will have an indicator stating "There have been recent commits to ```issuenumber-issue-branch-name```. Compare and Pull Request?"
- The button attached to that indicator will create a new PR!

This is where the important specification follow, so please follow this process closely. 

- Create a Draft Pull Request immediately. This starts the Github action [testing](###Tests) right away, and you won't have to wait 
- Edit the PR and fill out ALL of the relevant details. Thankfully, there is usually a template. Below is an example...
  - NOTE: If you use ```Fixes #issueNumber``` in your PR description your issue will automatically close when your branch is merged.
- Select a reviewer
  - All PR's require a reviewer. Try to rotate your reviewers so that everyone is familiar with multiple sections of the codebase 
- Await all [tests](###Tests) to pass and make sure they succeed
- If it is all green and succeeded, mark PR as Ready for Review!
- Update [project board](###ProjectBoard)

> Sometimes, we nail it on the first try. If your PR is approved, go ahead and merge your PR!

- Always use SQUASH AND MERGE. This keeps our commit history on ```main``` from getting out of control.

>Sometimes, we don't nail it on the first try, or the second, or the fiftieth, and thats okay. Some issues are hard. If you reviewer requests changes, you will have to review and make the changes, or discuss them with your reviewer. Essentially, you are reset to the top of the above list, except the pull request already exists. Any commits that you make to the issue branch will be recorded on the PR you already made. Make the changes, and rerequest a review when you are ready!

---

### Project Board

> Project board is a rather new feature to Github that Burmis uses to keep track of workflow on projects. 

Within the project board, you can find all of the same issues within the "[Issues](###Issues)" section of a repository. The main difference however, is the nice click and drag interface that lets us categorize tasks into different phases of developement. The interface is very self explanitory. Clicking on an [Issue](###Issues) will show more details about it, and you are able to click and drag them into different sections accordingly. Please keep this board up to date as you complete and move through tasks!

Some categories include... 

- ```Proposed``` (Not quite ready to start, but in the works.) 
- ```TODO``` (Ready to go! We are clear and ready for a developer to begin working on this issue.)
- ```Blocked``` (The worst! We have some sort of currently insurpassable blockage that prevents work on this issue.)
- ```In Progress``` (Whoever is listed as "Assigned" is currently working on this issue. Beat you to it!)
- ```Ready for Review``` (This issue currently has an open [PR](###PullRequests) that is awaiting review! Maybe yours!)
- ```Done``` (This task has been completed. Hooray!) 

As you move through your task list or issue, please return to and update this board accordingly. It helps keep everyone on the same page!

---
