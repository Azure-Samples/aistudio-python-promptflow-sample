# Azure AI Studio: Python PromptFlow Sample

This is the basic quickstart tutorial for the Azure AI Studio with PromptFlow. Find framework-specific versions here:
 - [Azure AI Studio SDK: Quickstart](https://github.com/Azure-Samples/aistudio-python-quickstart-sample)
 - [Azure AI Studio: Langchain Quickstart](https://github.com/Azure-Samples/aistudio-python-langchain-sample)

## 🧰 | Explore features of Azure AI Studio

The sample showcases features from the [Azure AI Studio preview](https://aka.ms/azureai/docs):

* [Azure AI Studio](https://aka.ms/azureaistudio/docs) - build, evaluate, deploy, your AI solution from one UI.
* [Azure AI Services](https://learn.microsoft.com/azure/ai-services/what-are-ai-services?WT.mc_id=academic-112432-pablolopes) - core AI Service APIs & Models usable in Azure AI Studio 
* [Azure AI SDK](https://learn.microsoft.com/azure/ai-studio/how-to/sdk-install?WT.mc_id=academic-112432-pablolopes) - for programmatic access to Azure AI Services.
* [Azure AI CLI](https://learn.microsoft.com/azure/ai-studio/how-to/cli-install?WT.mc_id=academic-112432-pablolopes) - for command-line access to Azure AI Services.

> [!WARNING]  
> Features contained in this repository are in private preview. Preview versions are provided without a service level agreement, and they are not recommended for production workloads. Certain features might not be supported or mvght have constrained capabilities. For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/?WT.mc_id=academic-112432-pablolopes).

## 👩🏽‍💻 | Build a copilot with your own data

Learn to build your own copilot using the Azure AI Studio with core resources (Azure AI Services) and tools (Azure AI SDK, Azure AI CLI). The tutorial guides you through the following steps:

1. Setup and validate your development environment.
2. Create an Azure AI project and AI resources for your copilot.
3. Create an Azure AI search index for your custom data.
4. Validate copilot by asking a question about your custom data.
5. Evaluate the performance of your copilot implementation. **Soon**
6. (Optional) Deploy the copilot to Azure and invoke it. **Soon**

## ✅ | Pre-Requisites

To work through this tutorial you will need:
1. Azure account with active subscription.
2. GitHub account with access to GitHub Codespaces.
3. (Optional) Set of docs that represent "your custom data".

The sample comes with a set of "product data" docs as default custom data. 

Make sure you have [access to the Azure AI Studio](https://learn.microsoft.com/en-us/azure/ai-studio/faq#how-can-customers-access-azure-ai-studio--?WT.mc_id=academic-112432-pablolopes) in your region, and can access related resources in your subscription. Refer to the [Azure AI Studio FAQ](https://learn.microsoft.com/en-us/azure/ai-studio/faq#how-can-customers-access-azure-ai-studio--?WT.mc_id=academic-112432-pablolopes) for more details on regional availability, pricing and more.

## 🏁 | Get Started

Ready to get started building a copilot with your own custom data? 

[**Start here**](./docs/promptflow/01-setup.md) to setup your development environment, then work through the remaining steps.

## 📚 | Relevant Resources

1. [Azure AI Studio](https://aka.ms/azureaistudio) - UI to explore, build & manage AI solutions.
1. [Azure AI Studio Docs](https://aka.ms/azureaistudio/docs) - Azure AI Studio documentation.
1. [Azure AI Services](https://learn.microsoft.com/azure/ai-services/what-are-ai-services?WT.mc_id=academic-112432-pablolopes) - Azure AI Services documentation.
1. [Training: Using vector search in Azure Cognitive Search](https://learn.microsoft.com/training/modules/improve-search-results-vector-searc?WT.mc_id=academic-112432-pablolopes) 
1. [Tutorial: Deploy a web app for chat on your data](https://learn.microsoft.com/azure/ai-studio/tutorials/deploy-chat-web-app?WT.mc_id=academic-112432-pablolopes) 