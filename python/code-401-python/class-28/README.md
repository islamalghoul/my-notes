[MainPage](../../../README.md)
# Next.js
New app Directory (Beta)
Today, we're improving the routing and layouts experience in Next.js and aligning with the future of React with the introduction of the app directory. This is a follow-up to the Layouts RFC previously published for community feedback.

The app directory is currently in beta and we do not recommend using it in production yet. You can use Next.js 13 with the pages directory with stable features like the improved next/image and next/link components, and opt into the app directory at your own pace. The pages directory will continue to be supported for the foreseeable future.

The app directory includes support for:

Layouts: Easily share UI between routes while preserving state and avoiding expensive re-renders.
Server Components: Making server-first the default for the most dynamic applications.
Streaming: Display instant loading states and stream in units of UI as they are rendered.
Support for Data Fetching: async Server Components and extended fetch API enables component-level fetching.
Server Components
The app/ directory introduces support for React's new Server Components architecture. Server and Client Components use the server and the client each for what they're best at - allowing you to build fast, highly-interactive apps with a single programming model that provides a great developer experience.

With Server Components, we're laying the foundations to build complex interfaces while reducing the amount of JavaScript sent to the client, enabling faster initial page loads.

When a route is loaded, the Next.js and React runtime will be loaded, which is cacheable and predictable in size. This runtime does not increase in size as your application grows. Further, the runtime is asynchronously loaded, enabling your HTML from the server to be progressively enhanced on the client.

Learn more about Server Components or deploy an example to try it out.

Streaming
The app/ directory introduces the ability to progressively render and incrementally stream rendered units of the UI to the client.

With Server Components and nested layouts in Next.js, you're able instantly render parts of the page that do not specifically require data, and show a loading state for parts of the page that are fetching data. With this approach, the user does not have to wait for the entire page to load before they can start interacting with it.

In the app directory, you can fetch data inside layouts, pages, and components – including support for streaming responses from the server.

We're enabling ergonomic ways to handle loading and error states and stream in UI as it's rendered. In a future release, we'll be improving and simplifying data mutations, as well.

