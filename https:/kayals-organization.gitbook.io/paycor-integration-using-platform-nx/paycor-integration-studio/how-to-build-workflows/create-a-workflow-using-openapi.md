# Create a Workflow using OpenAPI

#### <mark style="color:orange;">Step 01: Add a workflow</mark>

1. Select the application from the left-hand menu. Click on the **Application** folder, and then choose "**Workflows**." Inside the Workflows section, click on **Add a Workflow** to create a workflow for your application.

A create new workflow dialog will appear.

2. Select **OpenAPI.**

<mark style="color:orange;">**Step 02: Upload Specification**</mark>

2. In the "**Upload Specification**" section,&#x20;

**Option 1:**  Click or drag your OpenAPI specification file (in JSON or YAML format) into the provided area.

**Option 2:** Paste the API link as shown below:

Once the specification is uploaded, the system will parse and display available endpoints.

4. Click **Next**.

<mark style="color:orange;">**Step 3: Choose Endpoints**</mark>

5. Select the desired endpoints that you want to include in your workflow.
6. Click **Create**.
7. The system will process the selected endpoints and generate a new workflow based on the provided OpenAPI specification.
8. On the workflow creation page, edit the following details:
   * **Name** your workflow to clearly identify its purpose or function within the application.
   * Add the **description** for the workflow.

You can use these options to adjust the workflow.

* **Pointer**: This option allows you to access additional options about a selected node.
* **Hand**: Click and drag with the hand tool to navigate through the workflow, especially if the entire workflow is larger than the visible area.
* **Connector** - Use the connector tool to create connections or lines between nodes.
* **Color** - This option allows you to change the color of connectors, or other elements in your workflow.

5. Click **Save** to store the workflow configuration.

#### <mark style="color:orange;">Step 04: To configure trigger for the workflow</mark>

***

* Select a trigger for the workflow, such as a REST service.

<mark style="color:orange;">**Step 05: REST Service Configuration**</mark>

***

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.38.18 PM.png" alt=""><figcaption></figcaption></figure>

* Configure the REST service by providing details such as name, description, path, method, and media types.

<table><thead><tr><th width="216">Field</th><th>Description</th></tr></thead><tbody><tr><td>Name</td><td>The name to be displayed as the label for the activity in the process.</td></tr><tr><td>Description</td><td>Optional description of the activity purpose.</td></tr><tr><td>Path</td><td>The resource of the REST service.</td></tr><tr><td>Method</td><td><p>The REST methods used for the requests.</p><p>Select from one of the following available methods:</p><ul><li>POST</li><li>GET</li><li>PUT</li><li>DELETE</li></ul></td></tr><tr><td>Media Type</td><td><p>The value of the Content-Type header set while invoking the REST operation.</p><ul><li>JSON: the service provider returns the data in the JSON format.</li><li>XML: the service provider returns the data in the XML format.</li><li>Custom: to override the Content-Type value in the Input tab, select CUSTOM and provide the value in the Input tab.</li></ul></td></tr><tr><td></td><td></td></tr></tbody></table>

* **Headers:** Set up headers configuration, including name, default value, and enable/disable options for request and response
* **Path Parameters**: Define any dynamic values in your URL path that your service needs to process. These parameters help identify specific resources or actions in your service.
* **Query Parameters**: Add any additional parameters that modify your service's behavior, typically appended to the URL. These parameters can customize the response or filter the data your service returns.
* **Authentication (Auth)**: Specify how your service authenticates requests, like API keys or tokens. This ensures secure access and protects your service from unauthorized use.
* **Input Configuration (Source, Target, Mapping Expressions)**: Clarify where your service receives its input data and where it sends its output.

Use mapping expressions or functions to transform data between input and output formats.

* **Output Configuration**: Select a schema that outlines the structure of the data your service will return.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.40.52 PM.png" alt=""><figcaption></figcaption></figure>

Preview the output to confirm it aligns with your expectations and requirements.

* **Workflow Context:**

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.41.10 PM.png" alt=""><figcaption></figcaption></figure>

<mark style="color:orange;">**Step 04: Configure Response Activity**</mark>

***

Choose the response activity from the available activities.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.42.20 PM (1).png" alt=""><figcaption></figcaption></figure>

* Configure basic settings for the response activity, including input, source, target, and mapping expressions.
* Import the schema file or use the schema editor to define the schema.

<mark style="color:orange;">**Step 05: Publish Workflow**</mark>

***

* Once the workflow setup is complete, click on the "**Publish**" button located in the top-right corner.

<figure><img src="../../.gitbook/assets/Screenshot 2024-04-02 at 4.42.45 PM.png" alt=""><figcaption></figcaption></figure>

* Add a comment if necessary and click "**Publish**" to make the workflow available for deployment.

<mark style="color:orange;">**Step 06: Deploy Workflow**</mark>

***

After publishing, deploy your workflow to make it active and available for use.

* After publishing the workflow, click on the "**Deploy**" button.
* Specify the deployment details such as workflow name, environment, and version.
* Click "**Deploy**" to deploy the workflow.

After successful deployment, a success message will be displayed.

* The message will contain information such as version, build date, server URL, environment, and status.
* Click on the "**Promote**" button to proceed.

<mark style="color:orange;">**Step 07: Test API**</mark>

***

* Access the test page to verify the functionality of the deployed API.

Use the API testing feature to paste the request URL and configure authentication, parameters, headers, key, value, and body as needed.

* Test the API to ensure it works as expected.
