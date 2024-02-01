# Lab 3: Azure AI Studio Walkthrough

Azure AI Studio is a web-based platform that lets you build and manage AI applications using various tools and services. In this walkthrough, you will learn how to:

- Create an Azure AI resource and a project
- Use the prompt flow tool to generate text, speech, or images
- Deploy and consume a model from the model catalog
- Monitor and manage your AI resources and projects

## Exercise 1: Create an Azure AI resource and a project

1. Visit to <https://ai.azure.com/> and sign in  with your Azure account credentials.
1. On the home page, click on **Create a resource**.

1. Select a subscription, a resource group, a region, and a name for your Azure AI resource. You can also choose an Azure AI services provider, which determines the prebuilt AI models that you can access with your resource.

1. Click on **Review + create** and then **Create** to create your Azure AI resource. This may take a few minutes.

1. After your resource is created, you can see it on the **Manage** page. Click on **Create a project** to create a new project under your resource.
- Enter a name and a description for your project. You can also choose a project type, which determines the default tools and settings for your project. For this walkthrough, choose **General** as the project type.
- Click on **Create** to create your project. You will be redirected to the project page, where you can see the tools and components available for your project.

## Exercise 2: Use the prompt flow tool to generate text, speech, or images

1. On the project page, click on **Build** and then **Prompt flow** to open the prompt flow tool.

1. The prompt flow tool lets you generate text, speech, or images using large language models. You can choose from different scenarios, such as summarization, translation, image generation, and more.
1. For this walkthrough, let's try the **Text generation** scenario. Click on **Text generation** and then **Start**.

1. You will see a text box where you can enter a prompt, which is a piece of text that you want to continue or complete. For example, you can enter the beginning of a story, a question, or a sentence.
1. Enter a prompt of your choice and click on **Generate**. You will see the generated text below the prompt. You can adjust the parameters, such as length, creativity, and tone, to change the output. You can also click on **Generate** again to get a different output.

1. You can save the generated text by clicking on **Save**. You can also copy the text to the clipboard or share it with others by clicking on the corresponding icons.
1. You can try other scenarios, such as **Speech synthesis** , **Image generation** , and **Image captioning** , by clicking on the back arrow and selecting a different scenario.

## Exercise 3: Deploy and consume a model from the model catalog

1. On the project page, click on **Build** and then **Model catalog** to open the model catalog tool.

1. The model catalog tool lets you browse, deploy, and consume models that are fine-tuned or open-sourced by Microsoft or the community. You can choose from different domains, such as natural language processing, computer vision, speech, and more.

1. For this walkthrough, let's try the **Text summarization** model. Click on **Text summarization** and then **View details**.

1. You will see the details of the model, such as the description, the inputs, the outputs, and the performance metrics. You can also see a sample input and output, and try the model yourself by entering your own text and clicking on **Run**.
1. To deploy the model, click on **Deploy**.1. You will see a deployment wizard, where you can configure the deployment settings, such as the name, the compute target, the authentication, and the pricing tier.
1. Click on **Next** and then **Deploy** to deploy the model. This may take a few minutes.

1. After the model is deployed, you can see it on the **Deployments** page. You can also see the endpoint URL and the access key, which you can use to consume the model from your own applications.

1. To consume the model, you can use the **Test** tab, where you can enter an input and see the output. You can also use the **Code** tab, where you can see the code snippets for different languages, such as Python, C#, and JavaScript, to call the model endpoint.

## Exercise 4: Monitor and manage your AI resources and projects

1. On the project page, click on **Manage** to see the management tools and settings for your project. You can also go back to the **Manage** page of your Azure AI resource to see the management tools and settings for your resource.
1. The management tools and settings let you monitor and manage various aspects of your AI resources and projects, such as:
  - **Security** : You can configure the security settings, such as public network access, virtual networking, encryption, and privileged access, for your Azure AI resource and projects.
  - **Connections** : You can create and manage connections to external resources, such as data storage providers and Azure tools, for your Azure AI resource and projects.
  - **Compute and quota** : You can view and manage the compute resources and quota allocation for your Azure AI resource and projects.
  - **AI services** : You can view and manage the access keys and endpoints for the prebuilt AI models that are available for your Azure AI resource and projects.
  - **Policy** : You can view and manage the policy settings that are enforced on your Azure AI resource and projects.
  - **Dependent resources** : You can view and manage the dependent Azure resources that are used to store data and artifacts for your Azure AI resource and projects.
  - **Costs** : You can view and manage the costs and billing for your Azure AI resource and projects.

1. You can also use the **Settings** tab to change the name, description, and type of your project. You can also delete your project from there.


## Exercise 5: Test a text summarization

1. Navigate to Azure OpenAI Studio at <a href="https://oai.azure.com/" target="_blank">https://oai.azure.com/</a> and sign-in with credentials that have access to your OpenAI resource. During or after the sign-in workflow, select the appropriate directory, Azure subscription, and Azure OpenAI resource.
1. From the Azure OpenAI Studio landing page navigate further to explore examples for prompt completion, manage your deployments and models, and find learning resources such as documentation and community forums.
1. Start exploring Azure OpenAI capabilities with a no-code approach through the GPT-3 Playground. It's simply a text box where you can submit a prompt to generate a completion. From this page, you can quickly iterate and experiment with the capabilities.
1. You can select a deployment and choose from a few pre-loaded examples to get started. If your resource doesn't have a deployment, select **Create a deployment** and follow the instructions provided by the wizard. 
1. You can experiment with the configuration settings such as temperature and pre-response text to improve the performance of your task. 
- Selecting the **Generate** button will send the entered text to the completions API and stream the results back to the text box.
- Select the **Undo** button to undo the prior generation call.
- Select the **Regenerate** button to complete an undo and generation call together.

1. Azure OpenAI also performs content moderation on the prompt inputs and generated outputs. The prompts or responses may be filtered if harmful content is detected. 

1. In the GPT-3 playground you can also view Python and curl code samples pre-filled according to your selected settings. Just select **View code** next to the examples dropdown. You can write an application to complete the same task with the OpenAI Python SDK, curl, or other REST API client.

## Exercise 6: Try text summarization with GPT-3

To use the Azure OpenAI for text summarization in the GPT-3 Playground, follow these steps:

1. Sign in to [Azure OpenAI Studio](https://oai.azure.com).
1. Select the subscription and OpenAI resource to work with.
1. Select **GPT-3 Playground** at the top of the landing page.
1. Select your deployment from the **Deployments** dropdown. If your resource doesn't have a deployment, select **Create a deployment** and then revisit this step.
1. Select **Summarize Text** from the **Examples** dropdown.
1. Select `Generate`. Azure OpenAI will attempt to capture the context of text and rephrase it succinctly. You should get a result that resembles the following text:

    ```
    Tl;dr A neutron star is the collapsed core of a supergiant star. These incredibly dense objects are incredibly fascinating due to their strange properties and their potential for phenomena such as extreme gravitational forces and a strong magnetic field.
    ```

The accuracy of the response can vary per model. The Davinci based model in this example is well-suited to this type of summarization, whereas a Codex based model wouldn't perform as well at this particular task.

## Exercise 7: Clean up resources

If you want to clean up and remove an OpenAI resource, you can delete the resource or resource group. Deleting the resource group also deletes any other resources associated with it.