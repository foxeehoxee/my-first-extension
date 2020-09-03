# my-first-extension
A demo Azure DevOps web extension.


Creating a Web Extension (quick steps):
---------------------------------------
*Create an Organization
*Install Node
*Install extension packaging tool (TFX):
   npm install -g tfx-cli
*Initialize new NPM package manifest:
   npm init -y
*Install the Microsoft VSS Web Extension SDK package:
   npm install vss-web-extension-sdk --save
   (This SDK includes a JavaScript library that provides APIs required for communicating with the page your extension is embedded in.)
*Create an extension manifest file (i.e. => vss-extension.json) at extension root dir
*Create a view at extension root dir (i.e. => my-hub.html)

*Create a publisher in Visual Studio Marketplace Management Portal:
   https://marketplace.visualstudio.com/manage/publishers/markhawkes
   
*My First Extension:
   https://marketplace.visualstudio.com/items?itemName=MarkHawkes.my-first-extension
   
*Note your ID for the manifest file of extension (i.e. => MarkHawkes)
*Set the publisher in your manifest file (i.e. => MarkHawkes)
*Run the TFX tool's packaging command from your extension directory:
   tfx extension create
*Upload your newly created .vsix file in the management portal (new extension)
*Share with your organization
*View your extension in the marketplace and install it to your organization
*Select Organization settings, and then select Extensions to see your new extension:
   (Look for the "... More Actions" top-leftish menu)
   
   
Extension Building Checklist (from docs):
-----------------------------------------
1. Familiarize yourself with this article and the extension types already available within the Marketplace
    
    Extensions for Azure DevOps:
    https://marketplace.visualstudio.com/
    
2. Learn to build your first extension or check out our full set samples
    
    Build your first extension:
    https://docs.microsoft.com/en-us/azure/devops/extend/get-started/node?view=azure-devops
    
    Samples:
    https://docs.microsoft.com/en-us/azure/devops/extend/develop/samples-overview?view=azure-devops
    
3. Familiarize yourself with our RESTful APIs. If you're integrating from a third party app or service, you'll also want to check out our Service Hooks:
    
    REST APIs:
    https://docs.microsoft.com/en-us/rest/api/azure/devops/?view=azure-devops-rest-6.1&viewFallbackFrom=azure-devops
    
    Service Hooks:
    https://docs.microsoft.com/en-us/azure/devops/service-hooks/overview?view=azure-devops

4. Once your extension is ready, you'll want to package it, publish it to the Marketplace, and then we hope you'll share it with the community!
    
    Package, publish, and install your extension:
    https://docs.microsoft.com/en-us/azure/devops/extend/publish/overview?view=azure-devops    
        
    Package and publish your integration with an external app or service:
    https://docs.microsoft.com/en-us/azure/devops/extend/publish/integration?view=azure-devops    
        
    Share your work publicly with the entire community:
    https://docs.microsoft.com/en-us/azure/devops/extend/publish/publicize?view=azure-devops
 
 
