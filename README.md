# Host your resume in GitHub Pages

## Purpose
The purpose of this README is to explain how to host a resume on GitHub Pages. Also, this will introduce and demo principles of Andrew Etter's book _Modern Technical Writing_.

## Prerequisites
- GitHub account
- Resume formatted in Markdown

You will need to create a GitHub account to host your resume in GitHub Pages for free. Click [here](https://github.com/) to create an account.

Also, you will need to convert your resume into Markdown format. Don't worry if you are new to Markdown. There are websites that provides tutorials for beginners. I strongly recommend this [website](https://www.markdowntutorial.com/) to get yourself familar to Markdown then write your resume in Markdown.

## Instructions

### 1. Create a new repository on GitHub

By creating a new repository on GitHub, you are ready to use a distributed version control system (DVCS), Git. One of the Etter's protocol mentioned in his book is to use distributed version control to manage your remote repositories:

> "The basics are that DVCS have better performance, allow for offline work, [...] Atlassian BitBucket and Stash are both excellent web-based interfaces for managing remote repositories. GitHub and GitHub enterprise are also great options."

The good thing about using DVCS to manage your resume is you can do it in offline. If you need to download your resume and make a change, you can use Git to pull (download) it from the repository. 
Once the resume is editted, you can push (upload) it to the repository. Simple as that.

Let's create a new repository for your resume.

- On the top right corner, click **+** sign and **New repository**

![add_repo](./images/github_add_repo.PNG)

- Name your repository as _online-resume_
- Set it as **Public** (default)
- Check **Add a README file**
- Click **Crate repository**

![create_repo](./images/github_create_repo.PNG)

Your fresh repository for hosting resume should look like below.

![fresh_repo](./images/github_fresh_repo.PNG)

### 2. Choose a theme for your resume

You should try to make your resume look appealing and approachable. Etter mentions in his book that:

> "Whichever tool you select, take the time to customize the theme. [...] This customization is your chance to differentiate your content from the thousands of ugly, disorganized sites of the world, so don't just use the default theme."

Obviously, an uninteresting-looking resume won't attract anyone. Thankfully, you don't have to design the template of your resume by yourself. GitHub provides many built-in jekyll theme templates that look succint and professional. All you need to do is choose one of the jekyll themes that looks appealing to you (and others).

In case if you want to learn more about what jekyll is, click [here](https://jekyllrb.com/) to learn more about it.

Let's choose a theme for your resume!

- Click **Settings** of your repository

![pages_settings](./images/github_pages_settings.PNG)

- Scroll down and click **Pages** on the left navigation list

![pages_pages](./images/github_pages_pages.PNG)

- Click **Choose a theme**

![pages_none](./images/github_pages_none.PNG)

For this tutorial, we will use **Slate theme**.

- Click **Slate theme** (feel free to explore other themes, too)
- Then, click **Select theme**

![pages_slate](./images/github_pages_slate.PNG)

- Click **Commit changes**

![pages_slate_index](./images/github_pages_slate_index.PNG)

### 3. Enable GitHub Pages

GitHub Pages allows use to host a resume as a static website for free (but only one per account). Andrew Etter recommends to make a static website:

> "I love their speed, simplicity, portability, and security. You can host static websites practically anywhere, including Amazon S3 and GitHub Pages. They have no server-side application dependencies, no databases, and nothing to install, so migrating the entire site is as easy as moving a directory."

Static websites are fast. Like Etter stated, they do not consume hardware resources because no content is generated dynamically. 
By using GitHub Pages, you will be able see any change immediately on your resume (or **index.md**). It will be reflecetd in a few seconds (or minute, in the worst case). 

After the step 2, your repository will have a newly created a branch called **gh-pages** which contains **index.md** and **_config.yml** files. GitHub Pages should be enabled automatically as well.

To see if your GitHub Pages is up:
- Go to **Settings**
- Select **Pages** section on the left navigation list. 
- Click the link in the green box. 

![your_URL](./images/github_pages_URL.PNG)

The URL will look like the below format.

```
https://<github-username>.github.io/<repository-name>/
```

For my resume, the URL will be:
```
https://hyoungkyeu8359.github.io/online-resume/
```

### 4. Replace index.md with your resume

The reason why your resume should be written in Markdown format is because of it's easier to write and host in online platform. Etter explains why you should use Markdown:

> "Documentation should live online, and Word's abysmal HTML export is totally unsuitable for creating websites. [...] GitHub Flavoured Markdown is a popular and fine choice for simple web-based help systems."

Most people would use Microsoft Word to write their resume (and distribute PDF of their resume). However, as Etter stated in his book, .docx version of a resume is meant to be consumed and discarded. 

Writting a Markdown-formatted resume is easier to maintain and distribute in online. If you need to make a change to your resume, edit it, update the change to the repository, and it will stay fresh as new. Using Markdown is much simpler to write and easily distributable in GitHub Pages.

At this point, your website should contain default content. You will replace the content in **index.md** with your resume.

- Click **index.md** in your repository

![pages_index](./images/github_index.PNG)

- Click **Edit this file** (a pencil symbol)

![pages_index_edit](./images/github_index_edit.PNG)

- Replace the file with your resume
- Make sure to click **Preview** to see how your **index.md** will look like after change

![pages_index_edit2](./images/github_index_edit2.PNG)

- Click **Commit changes**

![pages_slate_index](./images/github_pages_slate_index.PNG)

## Verify your resume

Once **index.md** is modified, visit your GitHub Pages to see if your resume looks fine. Your website should look similar to below animation (as long as you are sticking with the **Slate theme**).

![demo](./images/demo.gif)

You can visit my resume at https://hyoungkyeu8359.github.io/online-resume/

Enjoy your resume!

## More resources

- Click [here](https://www.markdowntutorial.com/) for Markdown tutorial
- Click [here](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) to purchase Andrew Etter's book _Modern Technical Writing_ in Amazon
- Click [here](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages) for detailed documentation of GitHub Pages

## Authors and Acknowledgments:

GitHub Pages and the jekyll-theme-slate provided by GitHub was very helpful for hosting my resume.

Andrew Etter's protocols introduced in his book _Modern Technical Writing_.

Thanks to the members of Group 6 for reviewing my resume and README.md:
- Ryan Campbell
- Joshua Moreira
- Ikram Khan Shipon
- Anton Sikorsky

## FAQs 

**Q: Why is my resume not showing up?**

There are a few possibilities:
- Make sure your repository contains **index.md**
- You entered a wrong URL address.
- It takes a time to reflect any change you made in the repository. Keep refreshing the page!
- In the worst case, you might need to delete your repository and create a new one again.

**Q: Can I modify '_config.yml'?**

Yes. You may modify **_config.yml** to try something fancy in your resume. To see what you can add in **Slate** theme, please refer to this [repository](https://github.com/pages-themes/slate).

Please note that each theme have different configuration such that their **_config.yml** takes different variables. Make sure to check if your resume looks fine after modification.
