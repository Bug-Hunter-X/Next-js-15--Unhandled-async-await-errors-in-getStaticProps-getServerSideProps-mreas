# Next.js 15 Unhandled Async/Await Errors

This repository demonstrates a common error in Next.js 15 applications when using `async/await` within `getStaticProps` or `getServerSideProps`.  Improper error handling can lead to unexpected 500 Internal Server Errors, masking the root cause of the problem.  This example shows the issue and how to effectively handle it.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe the error in the browser console or Next.js logs (if applicable). 

## Solution

The solution involves proper use of `try...catch` blocks to wrap asynchronous operations and handle any potential errors gracefully.  The `bugSolution.js` file demonstrates this approach.

## Contributing

Contributions are welcome!  Feel free to open issues or submit pull requests.