---
layout: page-documentation-md
title: Edge Functions ChatGPT integration
description: The Azion Code Editor is integrated to the ChatGPT APIs, so you can use a set of features inside the editor, without opening another tab. The features go from refactoring the code to generating new code based on the prompt input.
meta_tags: edge, javascript
namespace: documentation_products_edge_functions_runtime_ai_integration
permalink: /documentation/products/edge-application/edge-functions/runtime-api/ai-integration/
permalink_pt-br: /documentacao/produtos/edge-application/edge-functions/runtime-api/ai-integration/
---

# Edge Functions ChatGPT integration

[ChatGPT](https://openai.com/blog/chatgpt) can be used in almost all tasks that involve understanding or generating natural language or code. In the development environment, it's a tool used for boosting developers productivity, helping them to:

- Explain the code being implemented.
- Generate new code.
- Refactor preexisting code.

---

## How does the Edge Functions ChatGPT integration work?

**Edge Functions Code Editor** is integrated to the ChatGPT APIs, so you can use a set of features inside the editor, without opening another tab. The features go from refactoring the code to generating new code based on the prompt input.

First, you need to configure your credentials registered on the OpenAI platform and generate an API key and org:

- [Generate ChatGPT API key](https://platform.openai.com/account/api-keys)
- [Generate ChatGPT Organization ID](https://platform.openai.com/account/org-settings)

With your credentials in hand, paste them into your source code as a comment, as exemplified below:

```javascript
    /*
    ChatGPTKey=key // Your ChatGPT key
    ChatGPTOrg=org // The org
    */
```

Now, with your credentials set, you're able to use the integration to develop faster and have your code reviewed whenever you like.

---

## Features

### Code Explanation

One feature available on this integration is **Code Explanation**. It comes in handy when you have to debug a function, or simply review it. It's also useful when you're working on legacy code.

### Code Generation

Code Generation works based on the prompt informed. For example, let's say you want to return an `HTML` page, with a table containing the name, phone number and address.

**Prompt**:
```javascript
    // generate an html table with name, phone number and address
```

After writing the prompt inside the code editor, right-click it and select `ChatGPT: Generate`.

**Output**:
```javascript
    <body>
     <table>
       <thead>
         <tr>
           <th>Name</th>
           <th>Phone Number</th>
           <th>Address</th>
         </tr>
       </thead>
       <tbody>
         <tr>
           <td>John Smith</td>
           <td>(123) 456-7890</td>
           <td>123 Main St, Anytown, USA</td>
         </tr>
         <tr>
           <td>Jane Doe</td>
           <td>(987) 654-3210</td>
           <td>456 Oak St, Anytown, USA</td>
         </tr>
         <tr>
           <td>Bob Johnson</td>
           <td>(555) 555-1212</td>
           <td>789 Maple St, Anytown, USA</td>
         </tr>
       </tbody>
     </table>
    </body>
```

### Code Refactor

Another option is to ask ChatGPT to refactor the code. To do so, you have to select the piece of code you want to have refactored, then right click on it and select `ChatGPT: Refactor`. After that, your code will be refactored automatically. 

Note that it's always a good idea to test and ensure the refactored code is working as expected, avoiding unexpected issues in the future.

---

## Implementation

Here are some real-life implementations of the Edge Functions ChatGPT integration:

| Implementation | Description   |
|---|---|
|  [How to build an API with Edge Functions and ChatGPT]()|See how to build an API and have its responses returned in JSON, with the help of ChatGPT |

---

## Related Documentation

- [Edge Functions Code Editor]({% tl documentation_products_edge_functions_runtime_code_editor %})
- [Azion Preview Deployment]({% tl documentation_products_edge_functions_runtime_ai_integration %})
- [Edge Functions - JavaScript Runtime APIs]({% tl documentation_products_edge_functions_runtime_apis_javascript %})
- [Edge Functions]({% tl documentation_products_edge_functions %})
- [Edge Functions on Edge Firewall]({% tl documentation_products_edge_functions_firewall %})

---

Didn’t find what you were looking for? [Open a support ticket](https://tickets.azion.com/).
