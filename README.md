1. Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

The best place to fit automated tests is within a GitHub Action that runs whenever code is pushed. This is so we ensure continuous and consistent feedback, allowing developers to catch and fix issues early in the development process. It also enforces code quality standards across all contributors by automatically running tests in a clean, controlled environment, unlike manually running tests locally—which can be forgotten or affected by differences in local setups—and running tests only after development is complete—which risks discovering bugs too late—integrating tests into a GitHub Action supports a more reliable and efficient workflow. This practice aligns with modern continuous integration and deployment (CI/CD) strategies and safer code delivery.

2. Would you use an end to end test to check if a function is returning the correct output? (yes/no)

No

3. What is the difference between navigation and snapshot mode?

Navigation mode: Analyzes the page load performance from the moment the page starts loading until it becomes interactive. It provides an overall performance score but does not track user interactions or dynamic content changes.

Snapshot mode: Analyzes the page in its current state (without reloading). It’s useful for checking accessibility and SEO issues but does not measure JavaScript performance or DOM changes over time.


4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.

  a. Add a \<meta name="viewport"\> tag – The report indicates that the page lacks a viewport meta tag, which is essential for responsive design on mobile devices.

  b. Improve cache policies for static assets – Lighthouse detected 5 resources that could benefit from better caching to speed up repeat visits.

  c. Reduce layout shifts – The report found one instance of a large layout shift, which can negatively impact user experience (CLS metric). Optimizing image dimensions or reserving space for dynamic content can help.





