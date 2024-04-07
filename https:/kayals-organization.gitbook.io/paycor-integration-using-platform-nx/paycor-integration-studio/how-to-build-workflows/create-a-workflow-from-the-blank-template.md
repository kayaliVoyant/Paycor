# Create a workflow from the blank template

#### <mark style="color:orange;">Step 01: Add a workflow</mark>

1. Select the application from the left-hand menu. Click on the **Application** folder, and then choose "**Workflows**." In the workflow section,  click **Add a Workflow** to create a new workflow for your application.

A create new workflow dialog will appear.

<figure><img src="../../.gitbook/assets/image (238).png" alt=""><figcaption></figcaption></figure>

2. Select **New.**

<figure><img src="../../.gitbook/assets/image (246).png" alt=""><figcaption></figcaption></figure>

2. On the workflow creation page, input the following details:

<figure><img src="../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

* **Name** your workflow to clearly identify its purpose or function within the application.
* Add the **description** for the workflow.

Your workflow canvas will automatically include a "**Start**" and "**End**" point by default, indicating the initial and final steps.

You can use these options to adjust the workflow.

* **Pointer**: This option allows you to access additional options about a selected node
* **Hand**: Click and drag with the hand tool to navigate through the workflow, especially if the entire workflow is larger than the visible area.
* **Connector** - Use the connector tool to create connections or lines between nodes.
* **Color** - This option allows you to change the color of connectors, or other elements in your workflow.

Click **Save** to store the workflow configuration.

***

#### <mark style="color:orange;">Step 02: To configure trigger for the workflow</mark>

* Select a trigger for the workflow, such as a REST service.

***

<mark style="color:orange;">**Step 03: REST Service Configuration**</mark>

* Configure the REST service by providing details such as name, description, path, method, and media types.

<figure><img src="../../.gitbook/assets/image (23) (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="216">Field</th><th>Description</th></tr></thead><tbody><tr><td>Name</td><td>Clear and descriptive name for the module.</td></tr><tr><td>Description</td><td>Optional description of the module's purpose.</td></tr><tr><td>Path</td><td>URL path or endpoint associated with the module.</td></tr><tr><td>Method</td><td>HTTP method(s) used to access the module (e.g., GET, POST).</td></tr><tr><td>Media Type</td><td>Format of data expected or returned by the module (e.g., JSON, XML).</td></tr></tbody></table>

* **Headers:** Set up headers configuration, including name, default value, and enable/disable options for request and response



* **Path Parameters**: Define any dynamic values in your URL path that your service needs to process. These parameters help identify specific resources or actions in your service.

<figure><img src="../../.gitbook/assets/image (25) (1).png" alt=""><figcaption></figcaption></figure>

* **Query Parameters**: Add any additional parameters that modify your service's behavior, typically appended to the URL. These parameters can customize the response or filter the data your service returns.



* **Authentication (Auth)**: Specify how your service authenticates requests, like API keys or tokens. This ensures secure access and protects your service from unauthorized use.
* **Input Configuration (Source, Target, Mapping Expressions)**: Clarify where your service receives its input data and where it sends its output.

Use mapping expressions or functions to transform data between input and output formats.

* **Output Configuration**: Select a schema that outlines the structure of the data your service will return.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.40.52 PM.png" alt=""><figcaption></figcaption></figure>

Preview the output to confirm it aligns with your expectations and requirements.

* **Workflow Context:**

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.41.10 PM.png" alt=""><figcaption></figcaption></figure>

***

<mark style="color:orange;">**Step 04: Configure Response Activity**</mark>

Choose the response activity from the available activities.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.42.20 PM (1).png" alt=""><figcaption></figcaption></figure>

* Configure basic settings for the response activity, including input, source, target, and mapping expressions.
* Import the schema file or use the schema editor to define the schema.

***

<mark style="color:orange;">**Step 05: Publish Workflow**</mark>

* Once the workflow setup is complete, click on the "**Publish**" icon located in the top-right corner.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.42.45 PM.png" alt=""><figcaption></figcaption></figure>

* Add a comment if necessary and click "**Publish**" to make the workflow available for deployment.

***

<mark style="color:orange;">**Step 06: Deploy Workflow**</mark>

After publishing, deploy your workflow to make it active and available for use.

* After publishing the workflow, click on the "**Deploy**" icon located in the top-right corner.
* Specify the deployment details such as workflow name, environment, and version.
* Click "**Deploy**" to deploy the workflow.

After successful deployment, a success message will be displayed.

* The message will contain information such as version, build date, server URL, environment, and status.
* Click on the "**Promote**" button to proceed.

***

<mark style="color:orange;">**Step 07: Test API**</mark>

* Access the test page to verify the functionality of the deployed API.

Use the API testing feature to paste the request URL and configure authentication, parameters, headers, key, value, and body as needed.

* Test the API to ensure it works as expected.

***
