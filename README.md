# How to merge your post

1. Fork the main repository [https://github.com/iclr-blog-track/iclr-blog-track.github.io](https://github.com/iclr-blog-track/iclr-blog-track.github.io).
3. Go to Settings -> Code and Automation -> Pages 

    ![image](https://user-images.githubusercontent.com/31974070/159055234-5ec4861e-87ca-459c-8093-ba9fd943d42c.png) 
    
    Take note of this URL!
    
    ![image](https://user-images.githubusercontent.com/31974070/159062054-2b29c739-16b9-4ec5-9ec1-3a9a549422be.png)

5. Select branch "master" in Source 

    ![image](https://user-images.githubusercontent.com/31974070/159055294-e38e9dc8-6053-4fe7-8a04-307272198403.png)
7. Go back to the main repository overview. Wait a few minutes for Github to populate the website.
8. Edit the url in `_config.yml`. To do so, simply comment out the old url, and add the one you obtained in step 2. 

    ![image](https://user-images.githubusercontent.com/31974070/159060707-6e6526ea-387c-4074-9102-76bcb540f9ed.png)
10. Upload your post and assets. Make sure everything renders correctly by visiting the url obtained in step 2. Take care to implement the changes requested by your reviewers if need be.
11. When you are ready to make your PR, create a branch named using your blog post's title. In this branch, undo your changes to the `_config.yml`. Create a PR from this new branch to the main repository's master branch. You can do so by cliking on the "Contribute" button. 

    ![image](https://user-images.githubusercontent.com/31974070/159061624-b0a85c3c-6ce1-4228-9178-cfc8185aef91.png) Voilà!
    
    Make sure that the base repository is the ICLR blog track's blog, and not `poole/lanyon` 
    
    ![image](https://user-images.githubusercontent.com/31974070/159993554-d762151f-3f7d-49af-a1b5-f62abdb5144e.png)

    As a sanity check, the only files changed in this PR should be your post and its assets.
    
    ![image](https://user-images.githubusercontent.com/31974070/159062613-120d572b-9300-46bc-9a52-05d3b84677d0.png)

12. We will then review your PR and merge it.
