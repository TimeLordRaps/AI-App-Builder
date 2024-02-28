# AI-App-Builder
This is the home of a self-assembling App that uses AI (Either openAI or langchain supported models) to build an app from the ground up from within the app.

# Plan
This will be a Next.js app that is capable of self-assembling.
It will have the following configurations:

"The dev": An app that is meant for someone familair with coding, probably even relative packages that are related to the project, but not necessarily. This version of the app will have the following features:
- Chat interface to directly converse with the app so that it can build itself.
- Code editor for directly modifying the source code of the application from within the application.
- Version control system that is able to render two separate versions of the application side by side, and/or in a slideshow manner where the user is able to quickly view different versions of the app as they are building it. The version control system will always maintain a stable working version and all relative changes from the default version that the AI and User made to the source code to get to the stable version, for purposes of easy control of the overall state of the app.

"The intern": An app that is meant for someone unfamiliar with code who still wants to experiment with AI and building apps via No-code. This verison of the app will have the following features:
- Chat interface to directly converse with the app so that it can build itself.
- Same verison control but the only changes being made are by the AI.

"The app": An instance of the app you made that doesn't have direct edit access. This will be more of a shipping process that prunes down the app you are working on to remove any functionality of the AI being able to directly edit source code, so that you may present your app to users. 

"The app" has whatever features you are able to add via direct modification of the source code of the template provided.

# Roadmap:
Create a basic working MVP of "The dev" by working on the features in the following order:

- code editor integration with @copilotkit.
- file system management by @copilotkit
- version control system basic level
- version control stable maintaince and changelog
- version control gui

After working on "The dev" I will simply remove the feautres based on the code editor to get "The intern".

Then start working on the shipping process so that the changelong from a default app template can be created into a functional app.

# Long term goals:
- Train a small model on the type of code that is generally used to edit apps via this method to create a shippable engine.
- Create a finetuning setup so that "dev"s and "interns"s can create finetunes of the types of models that would be interacting with their app's state based on a general telemetry setup.
