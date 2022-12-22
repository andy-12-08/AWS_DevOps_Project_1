Implementation of a continuous delivery pipeline for a simple web application. 
The following was implemented:
• Set up a GitHub repository to store the application code.
• Create the environment where the web application will be deployed using AWS Elastic Beanstalk.
• Configure and execute the build process for the application using AWS CodeBuild.
• Create a pipeline to automatically build and deploy the application using AWS CodePipeline.

Code Build was used here: It is important to note that build stage maybe needed or skipped, depending on your codebase.
on your code.

AWS CodeBuild is a fully managed build service that compiles source code, runs tests, and produces software packages that are ready to deploy. You might want to include a CodeBuild stage in your pipeline if you need to build, test, or package your code before deploying it.

Here are a few examples of when you might want to use CodeBuild in your pipeline:

If you have a multi-language codebase and need to build and package your code in a variety of languages.
If you want to run automated tests as part of your build process to ensure that your code is working correctly before deploying it.
If you need to create a deployable package (such as a JAR file, WAR file, or Docker image) as part of your build process.

On the other hand, you might want to skip the CodeBuild stage if you don't need to build or package your code before deploying it. For example, if you're deploying a static website that consists of HTML, CSS, and JavaScript files, you might not need to use CodeBuild since these files are ready to be deployed as-is. Ultimately, the decision to use CodeBuild in your pipeline will depend on the specific requirements of your project.
