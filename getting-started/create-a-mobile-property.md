# Setup a Mobile Property

Creating and configuring a mobile property is simple. Follow these steps to begin:

### Create a new mobile property

1. Click **New Property**
2. Create a new property by providing a name and selecting **Mobile** as the platform. If required, you may change [**Privacy** ](../resources/privacy-and-gdpr.md#setting-privacy-status)and **HTTPS** settings later.
3. Find the new property in the **Properties** list and click to open it.

### Setup Extensions

1. Setup **Extensions**
   1. Go to the **Extensions** tab. You should see that **Mobile Core** and **Profile** extensions are installed by default.  

   2. Click Configure on the **Mobile Core** card**.** 

      ![](../.gitbook/assets/screen-shot-2018-10-02-at-5.02.05-pm%20%282%29.png)

      1. Provide your Experience Cloud Org ID - This is a required identifier for your Experience Cloud Organization. This is typically, a 24-character, alphanumeric string followed by @AdobeOrg. If you need help finding it, contact your Adobe CSM or Customer Care.
      2. Optionally, provide your Experience Cloud ID Server - This is an optional server value which will be used to send Visitor ID Service network requests to a custom endpoint.
      3. Optionally, change the **Session Timeout** - A default value of 300 seconds is already set. This timeout value indicates the number of seconds that must pass after a user backgrounds the app before we consider an launch a new Lifecycle session.

   3. Hit **Save** to confirm your settings for **Mobile Core**.
   4. Click **Catalog**, and install all the extensions you need.

{% hint style="info" %}
Not sure on what extensions you need? Checkout the extensions listed in the **Using Mobile Extensions** section.
{% endhint %}

### Publish Configuration

Publish configuration In this step, you'll create library of changes and then deploy the library to a **Development Environment**.

1. In the **Publishing** tab, click on **Add New Library** under the **Development** section of the publishing workflow. 
2. Specify a name for the library and select a development environment from the **Environment** dropdown.
3. Add the configuration changes to be deployed.
4. Click **Add All Changed Resources** \(or to add only some changes, click **Add a Resource**\). 
5. Click **Save & Build for Development**. _Note: The library will build and then show under the **Development** section of the publishing workflow._
6. Click on the down arrow for the library and select **Submit for Approval**.

The configuration contained in the library will then be deployed to the Development environment and the library will show under the Submitted section of the publishing workflow.

{% hint style="info" %}
Testing can be done using the configuration in the Development environment. Later, the library can be deployed to **Staging** and **Production Environments** using the rest of the publishing workflow. Please see \(link-to publishing-to-stage/prod-here\)**.**
{% endhint %}
