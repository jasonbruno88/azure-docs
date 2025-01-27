---
author: ggailey777
ms.service: azure-functions
ms.topic: include
ms.date: 09/28/2020
ms.author: glenga
---

## Publish the project to Azure

In this section, you create a function app and related resources in your Azure subscription and then deploy your code.

> [!IMPORTANT]
> Publishing to an existing function app overwrites the content of that app in Azure.


1. Choose the Azure icon in the Activity bar, then in the **Azure: Functions** area, choose the **Deploy to function app...** button.

    ![Publish your project to Azure](./media/functions-publish-project-vscode/function-app-publish-project.png)

1. Provide the following information at the prompts:

    - **Select folder**: Choose a folder from your workspace or browse to one that contains your function app. You won't see this if you already have a valid function app opened.

    - **Select subscription**: Choose the subscription to use. You won't see this if you only have one subscription.

    - **Select Function App in Azure**: Choose `- Create new Function App`. By default, PowerShell app will be deployed to Windows Function App. If you want to use Linux Function app, choose the `Advanced` option.
      
    - **Enter a globally unique name for the function app**: Type a name that is valid in a URL path. The name you type is validated to make sure that it's unique in Azure Functions.
    
    - **Select a location for new resources**:  For better performance, choose a [region](https://azure.microsoft.com/regions/) near you. 
    
    The extension shows the status of individual resources as they are being created in Azure in the notification area.

    :::image type="content" source="media/functions-publish-project-vscode/resource-notification.png" alt-text="Notification of Azure resource creation":::
    
1.  When completed, the following Azure resources are created in your subscription, using names based on your function app name:
    
    [!INCLUDE [functions-vs-code-created-resources](functions-vs-code-created-resources.md)]

    A notification is displayed after your function app is created and the deployment package is applied. 

    [!INCLUDE [functions-vs-code-create-tip](functions-vs-code-create-tip.md)]

4. Select **View Output** in this notification to view the creation and deployment results, including the Azure resources that you created. If you miss the notification, select the bell icon in the lower right corner to see it again.

    ![Create complete notification](media/functions-publish-project-vscode/function-create-notifications.png)
