# How to merge your post

1. Fork the main repository [https://github.com/iclr-blog-track/iclr-blog-track.github.io](https://github.com/iclr-blog-track/iclr-blog-track.github.io).
2. Go to Settings -> Code and Automation -> Pages ![image](https://user-images.githubusercontent.com/31974070/159055234-5ec4861e-87ca-459c-8093-ba9fd943d42c.png) Take note of this URL!
3. Select branch "master" in Source ![image](https://user-images.githubusercontent.com/31974070/159055294-e38e9dc8-6053-4fe7-8a04-307272198403.png)
4. Go back to the main repository overview. Wait a few minutes for Github to populate the website.
5. Edit the url in `_config.yml`. To do so, simply comment out the old url, and add the one you obtained in step 2. ![image](https://user-images.githubusercontent.com/31974070/159060707-6e6526ea-387c-4074-9102-76bcb540f9ed.png)
6. Upload your post and assets. Make sure everything renders by visiting the url obtained in step 2. Take care to implement the changes requested by your reviewers if need be.
7. When you are ready to make your PR, create a branch named using your blog post's title. In this branch, undo your changes to the `_config.yml`. Create a PR from this new branch to the main repository's master branch. You can do so by cliking on the "Contribute" button. ![image](https://user-images.githubusercontent.com/31974070/159061624-b0a85c3c-6ce1-4228-9178-cfc8185aef91.png) Voilà!
