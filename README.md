# com_mapping-service-input



Mapping Component Overview:

The Mapping component serves as a user-friendly interface to extract metadata from data generated by instruments and map it to metadata schema.Our mappings are designed to align with widely accepted community schemes, custom-tailored for various techniques.

## Integration

If the dependency is up set properly (instructions will follow), the component can be used like this:

**Add the Element**:
To integrate the Mapping component into your project, insert the following HTML element into your webpage:

```html
<head>
     ...
    <!-- add the below code !-->
     <script src="https://cdn.jsdelivr.net/npm/@kit-data-manager/mapping-service-input@latest/dist/com_mapping-service-input.es.js"></script>
</head>
<body>
    <!-- use the component !-->
    <mapping-input base-url="http://localhost:8090/" id="input-component"></mapping-input>
</body>
```
**Invoke the Download Functionality**:

For enabling the download functionality, include the following HTML code in your page:
```html

`<div class="ui center aligned grid">
  <button type="submit" class="ui primary button" id="submit" onclick="
    var component = document.getElementById('input-component');
    component.executeMapping(true)">Map document
  </button>
</div>`

```

The executeMapping(true) method call triggers both the mapping process and the subsequent download of the result.

Adjusting Base URL:
The base-url attribute in the <mapping-input> element allows you to specify the base URL for your Mapping Service instance. You can modify this URL as needed to suit your requirements.

By following these steps, you can easily integrate the Mapping component into your project and utilize its capabilities for extracting metadata from instrument-generated data.


## How to run - For developers

To start using the component clone this repo to a new directory:

```bash
git clone https://github.com/kit-data-manager/com_mapping-service-input.git
```

and run:(Before running below command make sure node.js is installed in your system. You can check if it is there is your system or not by command: node -v or node --version (dependending on the operating system you are using) in your command prompt.

```bash
npm install
```

To runthe component in developement mode

```bash
npm run build
npm run dev
```

DONOT forget to add the html code(mentioned above) to run this locally.


## Attributes

- `base-url`: string, base-url to your Mapping Service instance


## Methods
- `executeMapping(true)`: To trigger the mapping process, you can include the following HTML code in your project:
 (true in the method argument will trigger mapping + download of the result)





  
