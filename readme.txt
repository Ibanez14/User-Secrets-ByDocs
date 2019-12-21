USER SECRETS

Environment variables are used to avoid storage of app secrets in code or in local configuration files.
Environment variables override configuration values for all previously specified configuration sources.




1) Add in csproj a GUID
<UserSecretsId>79a3edd0-2092-40a2-a04d-dcb46d5ca9ed</UserSecretsId>

OR

1) In Visual Studio, right-click the project in Solution Explorer, 
and select Manage User Secrets from the context menu. This gesture adds a U
serSecretsId element, populated with a GUID, to the .csproj file.


OR

build project and type

dotnet user-secrets init


Add, edit values
----------------------------------

2) Add, edit via Visual studio in json file directly 

OR
via CLI

dotnet user-secrets set "key" "value"
dotnet user-secrets list
dotnet user-secrets remove "key"
dotnet user-secrets clear // deletes all
