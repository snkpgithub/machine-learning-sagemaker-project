# Machine Learning SageMaker Project
### Generative AI Labs and Model Deployments using AWS SageMaker

This project is inspired by the AWS Immersion Day format and is aimed at helping users get started with Generative AI using AWS services, especially SageMaker. It is structured into four main modules, each combining theoretical background (via slides) and practical hands-on labs (via Jupyter notebooks).

### 🧠 Modules Included:
1. **Introduction to Generative AI & Large Language Models**
   - Model deployment and inference optimization
2. **Finetuning Large Language Models**
3. **Visual Foundation Models**
   - Stable Diffusion deployment and inference
4. **Building GenAI Applications**
   - Engineering GenAI-powered apps using Retrieval-Augmented Generation (RAG)

> Note: During workshops or personal learning sessions, you may choose to cover only a subset of these modules.

---

### 📁 Repository Structure:

- 📊 **Slides**:  
  `GenerativeAIImmersionDayPresentationDeck.pdf` — Available at the root of the repository

- 🔬 **Lab 1: Hosting Large Language Models** (`lab1/`)  
  - Option 1: GPT-J → `option-1-gpt-j-notebook-full.ipynb`  
  - Option 2: Falcon40B-Instruct → `falcon40b-instruct-notebook-full.ipynb`

- 🛠️ **Lab 2: Finetuning LLMs** (`lab2/`)  
  - Start with → `fine-tuning.ipynb`

- 🎨 **Lab 3: Hosting Stable Diffusion** (`lab3/`)  
  - Start with → `JumpStart_Stable_Diffusion_Inference_Only.ipynb`

- 🤖 **Lab 4: Building AWSomeChat using RAG** (`lab4/`)  
  - Start with → `rag-app.ipynb`

---

### 🧰 Prerequisites:
To conduct the labs successfully, make sure your AWS account is properly set up. This includes permissions for using SageMaker, S3, and related services. Configuration details are provided in the setup section of each lab.

---

Let me know if you'd like me to:
- Add a logo/banner
- Make a `setup.md` or `CONTRIBUTING.md` file
- Add badges (build, license, etc.)


# Setup

## AWS-hosted event

### Event Engine AWS Account access

[Click here](https://catalog.workshops.aws/join), paste in the access code and log in to the AWS Workshop Portal to proceed with the lab. 

Click Email One-Time Password (OTP) button.

![Sign In](./img/3-sign-in.png)

Write down your own email account and click the Send passcode button.

![Passcode](./img/3-one-time-passcode.png)

In your email inbox, check for the email subject "Your one-time passcode email" and copy the passcode. Paste the copied passcode as shown below, then press the Sign in button.

![Passcode 2](./img/3-one-time-passcode-2.png)

Enter the 12-character Event Access Code received from the event organizer and click Next.

![Event Access Code](./img/3-event-access-code.png)

Read Terms and Condition and accept by selecting I agree with the Terms and Conditions. Click Join event.

![Terms and Conditions](./img/3-terms-and-condition.png)

In the next window that appears, click the Open AWS Console button. Note, that the workshop content and region can vary depending on your specific event.

![Terms and Conditions](./img/3-test-event.png)

The AWS Console will open in a new browser window.

![Terms and Conditions](./img/3-event-generator-aws-console-3.png)

If you see the following message, your browser has been previously logged into another AWS account.

Click the **"here"** link to logout of your AWS Console, go back to click on "*Open AWS Console*" button.

![Terms and Conditions](./img/3-event-generator-aws-console-signout.png)

Amazon SageMaker Studio Access: Amazon SageMaker Studio is a web-based, integrated development environment (IDE) for machine learning that lets you build, train, debug, deploy, and monitor your machine learning models. Studio provides all the tools you need to take your models from experimentation to production while boosting your productivity.

If the AWS Account has been provisioned by your AWS Instructor, follow the next steps to access the SageMaker Studio environment:

Open AWS console and switch to AWS region communicated by your instructor. 

You can find the list of the AWS regions that support SageMaker Studio [here](https://docs.aws.amazon.com/sagemaker/latest/dg/studio.html).

![Management Console](./img/mgmtConsole.png)

Under services search for Amazon SageMaker.

![SageMaker](./img/sagemaker.png)

Under Get Started, click on the orange button SageMaker Studio.

![SageMaker Studio](./img/sagemakerStudio.png)

A SageMaker Studio environment should already be provisioned. Click on Open Studio (on the right side of the preprovisioned sagemakeruser username).

![SageMaker Domain](./img/sagemakerDomain.png)

The page can take 1 or 2 minutes to load when you access SageMaker Studio for the first time.

![SageMaker loading](./img/sagemakerLoading.png)

You will be redirected to a new web tab that looks like the below figure. Click Open Launcher.

![SageMaker start](./img/openLauncher.png)

Under Notebooks and compute resources, make sure that the Data Science SageMaker image is selected and click on Notebook - Python 3.

![Notebooks & Compute resources](./img/notebooksComputeResources.png)

You will land in the Untitled.ipynb notebook.

![Untitled](./img/untitled.png)

You can rename the notebook by right clicking on the name.

![Rename](./img/rename.png)

![Rename file](./img/renameFile.png)

Congratulations!! You have successfully launched a SageMaker Studio Notebook and are now familiar with the basic flow within Sagemaker Studio. You will not need this specific notebook for the upcoming labs, however you can use the exact same notebook configuration (instance, image) throughout the upcoming labs.

# Downloading the content of the GitHub repository needed for the labs

## Clone Repository

```console
!git clone https://github.com/aristsakpinis93/generative-ai-immersion-day
```

After completion of step 2 you will have llm-immersion-day folder created in left panel of the studio:

![Cloned repo](./img/cloned.png)

Congratulations!! You have successfully downloaded the content of the Generative AI Immersion Day. From now on you can start working on the labs! 

Lab 1 - Hosting Large Language Models can be found in the lab1 directory. 
- Option 1: For GPT-J start with the notebook option-1-gpt-j-notebook-full.ipynb.
- Option 2: For Falcon40b-instruct start with the notebook falcon40b-instruct-notebook-full.ipynb.
Lab 2 - Finetuning Large Language Models can be found in the lab2 directory. Start with the notebook fine-tuning.ipynb.
Lab 3 - Hosting Stable Diffusion can be found in the lab3 directory. Start with the notebook JumpStart_Stable_Diffusion_Inference_Only.ipynb.
Lab 4 - Building the LLM-powered chatbot "AWSomeChat" with retrieval-augmented generation. Start with the notebook rag-app.ipynb.
