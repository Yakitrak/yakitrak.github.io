# Resume

Repository to keep and deploy my resume in JSON, HTML and PDF format.

## View it

- HTML on [kjainwal.com](https://kjainwal.com/)
- PDF on [kjainwal.com/resume.pdf](https://kjainwal.com/resume.pdf)
- JSON on [kjainwal.com/resume.json](https://kjainwal.com/resume.json)

## Motivations

I used [JSON-Resume](https://jsonresume.org/) to create my resume. This means I won't be creating my resume or portfolio every year! Instead, I could focus on the content on a simple JSON file and simply change or create a new theme when I want. It is also easy to keep it updated and deployed with Github pages.

Now you may be wondering why not use the hosted solution already provided by JSON-Resume? Here is my reasoning:

- Central repository to keep my resume in all 3 versions (JSON, HTML and PDF) whereas JSON-Resume only hosts the HTML
- More contol over themes (currently using my own [caffeine-tweaked](https://www.npmjs.com/package/jsonresume-theme-caffeine-tweaked) theme from the original [caffeine](https://www.npmjs.com/package/jsonresume-theme-caffeine) theme)
- Can use custom domain

## Build

```
nvm use 12.0.0 
```

```
resume export --resume docs/resume.json --theme jsonresume-theme-caffeine-tweaked --format html docs/index.html
```

Replace paths and theme arguements as needed
