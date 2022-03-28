# How to merge your post

The high level process of merging your post is to fork [our repository](https://github.com/iclr-blog-track/iclr-blog-track.github.io), add your blog post markdown file with the assets, and then open a pull request against our master branch. 
We additionally provide optional instructions for hosting github pages on your own github account in order to preview your post before submitting the pull request, but this is not required if you don't wish to preview the pages.

## Merging your contributions

1. **Fork the main ICLR blog track repository**: [https://github.com/iclr-blog-track/iclr-blog-track.github.io](https://github.com/iclr-blog-track/iclr-blog-track.github.io).
    Create a branch where you will be staging all of your content for the pull request.

2. (Optional*) If you wish to preview your posts before making a pull request, you can follow the 
    instructions provided in [Previewing your blog posts](#optional-previewing-your-blog-posts) 
    section to setup github pages on your fork.
    This is strictly for debugging purposes and is not required if you wish to just proceed with a pull request. 
    **Note: if you follow these steps, we ask that you take down the hosted site when you're done with the pull request to avoid any potential confusion with the official ICLR site.*

3. **Upload your post and assets.** 
    **Ensure you implemented any of the changes/modifications requested by the reviewers on OpenReview**.
    As a reminder, your contributions should be:
    
    - Your blog post in `_posts/2022-03-25-[YOUR SUBMISSION].md`
    - (Optionally) any static images must be in `public/images/2022-03-25-[YOUR SUBMISSION]/`
    - (Optionally) any HTML content must be in `_includes/2022-03-25-[YOUR SUBMISSION]/`
    
    where `2022-03-25-[YOUR SUBMISSION]` is the same string across the blog post file and two directories (note the updated date).
    Any other changes in your pull request will be rejected and you will be asked to modify your PR accordingly.
    Visually, we expect the changes to look like the following:
    ```bash
    iclr-blog-track.github.io/
    │
    ├── _includes
    │   ├── 2022-03-25-[YOUR SUBMISSION]         # <--- Directory containing of any HTML figures (if necessary)
    │   │   └── [YOUR HTML FIGURES].html
    │   └── ...
    ├── _posts
    │   ├── 2022-03-25-[YOUR SUBMISSION].md      # <--- Your actual post (required)
    │   └── ...
    ├── public
    │   ├── images
    │   │   ├── 2022-03-25-[YOUR SUBMISSION]     # <--- Directory containing any static images (if necessary)
    │   │   │   └── [YOUR IMAGES].png
    │   │   └── ...
    │   └── ...
    └── ...
    ```

    
    

4. **Create a pull request to our repo's master branch.**
    You can do so by clicking on the `Contribute` button. 

    ![image](https://user-images.githubusercontent.com/31974070/159061624-b0a85c3c-6ce1-4228-9178-cfc8185aef91.png)
    
    ***CRITICAL***: **make sure that the base repository is the ICLR blog track's blog, and not `poole/lanyon`!**
    
    ![image](https://user-images.githubusercontent.com/31974070/159993554-d762151f-3f7d-49af-a1b5-f62abdb5144e.png)

    Please name your PR with the format: `[OPENREVIEW #] - [POST TITLE]`, for example: `100 - Towards Deep Learning Blog Posts`.
    Please use the pull request template provided.
    It should automatically populate your pull request, and look like the following:
    ```
    ## OpenReview Submission Thread

    - [url to your submissions Openreview thread]

    ## Checklist before requesting a review
    - [ ] I have followed the instructions and have only added changes as specified in the submission instructions (blog post and asset directories with correct naming scheme)
    - [ ] I have implemented the necessary changes in response to reviewer feedback
    - [ ] (optional, for tracking) I deployed github pages on my fork in order to preview my post
        - [ ] If yes, I have deleted my hosted github page once this pull request was closed (to be completed upon closing this PR)

    ## Changes implemented in response to reviewer feedback

    - n/a

    ## Any other comments

    - n/a
    ```
    As a sanity check, the only files changed in this PR should be your post and its assets.
    
    ![image](https://user-images.githubusercontent.com/31974070/159062613-120d572b-9300-46bc-9a52-05d3b84677d0.png)


12. We will then review your PR and merge it.


## (Optional) Previewing your blog posts 

To help you verify that your blog post will render correctly, you can host the blog post page on your own github account.
Follow these steps after forking our repository:

1. Go to `Settings` -> `Code and Automation` -> `Pages` 

    ![image](https://user-images.githubusercontent.com/31974070/159055234-5ec4861e-87ca-459c-8093-ba9fd943d42c.png) 
    
2. Select branch "master" in Source dropdown; doing so will provide you with a URL upon success.
    **Take note of this URL!**

    ![image](https://user-images.githubusercontent.com/31974070/159055294-e38e9dc8-6053-4fe7-8a04-307272198403.png)

3. Go back to the main repository overview. 
    Wait a few minutes for Github to populate the website.

4. Edit the `url` parameter in `_config.yml`. 
    You can comment out the old url and add the one you obtained in step 2. 

    ![image](https://user-images.githubusercontent.com/31974070/159060707-6e6526ea-387c-4074-9102-76bcb540f9ed.png)

5. When you are ready to make your PR, create a branch named using your blog post's title. 
    In this branch, undo your changes to the `_config.yml` as we do not want these changes in our own repo.

6. To delete your published site, change the branch `Source` that you specified in step 2 to `None`. 
