# DBE-.NET-Manage-Resource-Group

To run this sample for creating storage account:
1.	Clone the repository using the following command:
  ```
    git clone https://github.com/sijuman/DBE-Manage-Resource-Group.git
  ```
2.	Set the following required environment variable values:
      ```
    	AZURE_TENANT_ID
    	AZURE_SUBSCRIPTION_ID
    	ARM_ENDPOINT
    	RESOURCE_LOCATION	
        AZURE_USERNAME
    	AZURE_PASSWORD
      ```
3.	Change directory to sample:
    ```
	cd hybrid-storage-dotnet-manage-storage-accounts
    ```
4.	Ensure that the packages.config resembles below as it will use .NET framework as .NET core does not support username/password authentication yet.
    ```
	  <package id="Microsoft.Azure.Management.Profiles.hybrid_2018_03_01.ResourceManager" version="0.9.0-preview" targetFramework="net461" />
	  <package id="Microsoft.Azure.Management.ResourceManager.Fluent" version="1.27.0" targetFramework="net461" />
	  <package id="Microsoft.IdentityModel.Clients.ActiveDirectory" version="4.3.0" targetFramework="net461" />
	  <package id="Microsoft.IdentityModel.Logging" version="1.1.2" targetFramework="net461" />	  <package id="Microsoft.IdentityModel.Tokens" version="5.1.2" targetFramework="net461" />
	  <package id="Microsoft.Rest.ClientRuntime" version="2.3.19" targetFramework="net461" />
	  <package id="Microsoft.Rest.ClientRuntime.Azure" version="3.3.18" targetFramework="net461" />
	  <package id="Microsoft.Rest.ClientRuntime.Azure.Authentication" version="2.4.0" targetFramework="net461" />
	  <package id="Newtonsoft.Json" version="10.0.3" targetFramework="net461" />
    ```
5.	Run the sample:
  ```
	dotnet restore
	dotnet run
  ```

6.	The logs will show the storage account created as well as the name if the process was successful.
