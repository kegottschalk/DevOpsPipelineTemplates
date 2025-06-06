# DevOps Pipeline Templates
A collection of Azure DevOps Pipelines generic templates for building, packaging, and deploying various types of artifacts.

## Templates
- **template_archive_publish** - Template should be used to archive and publish files. Used for simple HTML websites, etc, that are not built but we need to publish an archive for deployment.
- **template_asp_net_build_publish** - Template should be used to build and publish a ASP.NET web app. Template will First call the NuGet template to install and download nuget packages. Then it will Build the VS solution. Finally will publish the build artifact.
- **template_console_app_deploy** - Template will download, configure, and deploy a .NET console app. Has support for a pre- and post- PowerShell script (optional).
- **template_iis_website_deploy** - Template will download, configure, and deploy an IIS Website. Has support for both XML and JSON based custom configs.
- **template_json_config_transform** - This template will modify JSON config files (i.e. appsettings.json).
- **template_nuget_restore** - This template will handle the NuGet Install / Restore commands.
- **template_pbi_item_deploy** - For Power BI / Fabric Project Files (.pbip). Template will download Power BI artifact then publish the Power BI item to the specified workspace.
- **template_publish_artifacts_generic** - Template will copy specified files and publish them as a Build Artifact.
- **template_sql_database_deploy** - Intended for on-prem or VM-based SQL Servers. Template will download Dacpac file, update DB using sqlpackage, then publish deploy results files. Optionally, can create Deploy Report only without upgrading the DB.
- **template_ssis_build_publish** - Template will Build an SSIS project and publish the artifacts. Requires extension "SSIS DevOps Tools" from Microsoft.
- **template_ssis_deploy** - Template will download and deploy an SSIS Project, then configure the Environment. Requires extension "SSIS DevOps Tools" from Microsoft.
- **template_synapse_wks_deploy** - Template will download json template artifacts and then deploy the Synapse Workspace.
- **template_vs_build** - Template will First call the NuGet template to install and download nuget packages. Then it will Build the VS solution.
- **template_vs_framework_build_publish** - Template should be used to build and publish a .NET Framework application. Template will First call the NuGet template to install and download nuget packages. Then it will Build the VS solution. Finally will publish the build artifact.
- **template_vs_publish** - Template will Publish a VS project and then retain the results as a Pipeline artifact.
- **template_xml_config_transform** - This template will transform XML config files (i.e. App.config). Requires a corresponding release config file (i.e. App.Release.config), that has XML transformation syntax. https://learn.microsoft.com/en-us/previous-versions/aspnet/dd465326(v=vs.110)

