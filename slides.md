---
theme: default
background: ./images/entrance_1.jpg
class: text-center
highlighter: shiki
lineNumbers: false
info: Presentation for ITZ 2023 Conf
drawings:
  persist: false
transition: slide-left
title: Welcome
mdc: true
---

# What your teachers don’t want you to know

My experience with collaboration and tools at Silicon Valley

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/interactivelabs/itz-presentation-2023" target="_blank" alt="GitHub"
    class="text-xl slidev-icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
  WELCOME
-->

---
layout: two-cols-header
transition: fade-out
level: 2
---

# Who am I?

::left::

## Luis Gonzalez

- <mdi-school-outline class="bg-gradient-to-r from-violet-500 to-sky-500" /> **ITZ Alumni** - Graduated 2004
- <fluent-mdl2-family class="bg-gradient-to-r from-pink-500 to-violet-500" /> **Husband and Father of 2** - Dulce, Robe & Eli
- <material-symbols-videogame-asset-outline class="bg-gradient-to-r from-violet-500 to-red-500" /> **Video game enjoyer** - Obsesced with Hades
- <icon-park-outline-laptop class="bg-gradient-to-r from-blue-500 to-violet-500" /> **Sr. Software Engineer** - Working at Airbnb

::right::

<div class="relative flex justify-center h-96">
  <img v-click="[1,2]" src="/images/sold_school.jpg" class="h-96 absolute" />
  <img v-click="[2,3]" src="/images/family.jpg" class="h-96 absolute" />
  <img v-click="[3,4]" src="/images/hades_cover.jpg" class="h-96 absolute" />
  <img v-click="[4,5]" src="/images/luis_bar_1.jpg" class="h-96 absolute" />
  <img v-click="[5,6]" src="/images/office_1.jpg" class="h-96 absolute" />
  <img v-click="6" src="/images/me_office_1.jpg" class="h-96 absolute" />
</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
  INTRO
-->

---
layout: cover
background: https://source.unsplash.com/collection/1134422/1920x1080
level: 2
---

# Disclaimer

---
layout: default
level: 2
---

# Table of contents

<Toc maxDepth="1"></Toc>

---
layout: two-cols-header
transition: slide-up
---

# What do I do?

Why the title of the presentation?

::left::

<v-clicks depth="2">

- Writing code for a living
- Finding Solutions
  - **Learning**
  - **Understanding Code**
    - Read and interpret documentation
  - Debug issues

</v-clicks>

::right::

<div class="relative flex justify-center h-96">
  <img v-click="[1,2]" src="/images/why_works.png" class="h-96 absolute" />
  <img v-click="[4,5]" src="/images/docs_meme.png" class="h-96 absolute" />
  <img v-click="[5,6]" src="/images/progress.webp" class="h-96 absolute" />
</div>

<!--
  EXPLAIN WHY ME AND WHY I BELIEVE THIS NEEDS TO BE ADDRESSED
-->

---
layout: cover
background: ./images/entrance_2.jpg
---

# **Collaboration** and Tools

---
layout: image-right
image: /images/kitchen_1.jpg
level: 2
---

# Project Management

- (Un)Agile
  - Projects
  - Maintenance
  - Migrations
- Team Structures
  - By Product/Surface
  - By Dicipline

<!--
  HOW DO WE ORGINIZE
-->

---
layout: image-left
image: /images/kitchen_2.jpg
level: 2
---

# Developing the code

- Containers for local development
- Automated Testing
  - Linters and Formatters
  - Unit Testing
  - Integration Testing
  - E2E Testing

<!--
  CODING
-->

---
layout: image-left
image: /images/docker.png
level: 3
---

# Containers for local development

<img src="/images/docker_dev_env.png" />

<!--
  CODING
-->

---
layout: image-left
image: /images/entrance_1.jpg
level: 3
---

# Automated Testing

- Linting and Formatting
  - <logos-prettier /> Prettier
  - <logos-eslint /> ESLint

<img src="/images/prettier.gif" />

- Unit Testing

```javascript
function sum(a, b) {
  return a + b;
}

test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3);
});
```

<!--
  CODING
-->

---
layout: image-left
image: /images/entrance_2.jpg
level: 3
---

# Automated Testing

- Integration Testing

```javascript
[TestFixture]
public class MyServiceIntegrationTests
{
  [Test]
  public async Task MyService_ReturnsOk()
  {
    var response = await _client.GetAsync("/api/myservice");
    // Assert that the response status code is 200 OK
    response.EnsureSuccessStatusCode();
  }
}
```

- E2E Testing

```javascript
describe('My Page', () => {
  it('should have a button', () => {
    cy.visit('/my-page');
    cy.get('button').should('exist');
  });
});
```

<!--
  CODING
-->

---
layout: image-right
image: /images/office_1.jpg
level: 2
---

# Code Collaboration

- Version Control (Git)
  - <mdi-github /> GitHub
  - <logos-gitlab /> GitLab

1. Clone the repository to your local machine:

```bash
gh repo clone <repository>
```

2. Create a new branch for your feature or bug fix:

```bash
git checkout -b <branch-name>
```

3. Make changes to the code and commit them:

```bash
git add .
git commit -m "Your commit message"
```

<!--
  SHARING THE CODE
-->

---
layout: image-right
image: /images/office_1.jpg
level: 2
---

# Code Collaboration

4. Push your changes to the remote branch:

```bash
git push -u origin <branch-name>
```

5. Open a pull request on GitHub:

```bash
gh pr create --title "Your pull request title" --body "Your pull request description"
```

6. Review and discuss the changes with your team and make any necessary updates to the code.
7. Once the pull request is approved, merge it into the main branch:

```bash
gh pr merge <pull-request-number> --merge
```

8. Delete the remote branch:

```bash
gh pr close <pull-request-number>
```

<!--
SHARING THE CODE
-->

---
layout: image-right
image: /images/docs.png
level: 2
---

# Code Collaboration

- Documentation
  - <simple-icons-nextra /> https://nextra.site
- Service Discovery
  - <cib-swagger /> Swagger

<img v-click="1" src="/images/swagger.png" />

<!--
SHARING THE CODE
-->

---
layout: image-right
image: https://source.unsplash.com/collection/1134422/1920x1080
level: 2
---

# Code Deployment

- Cloud services
  - <logos-aws /> AWS
  - <logos-google-cloud/> Google Cloud
  - <logos-microsoft-azure /> Azure
  - <radix-icons-vercel-logo class="color-white" /> Vercel
- Cloud Offerings
  - Edge
    - <logos-aws-lambda /> AWS Lambda
  - Containers
    - <logos-aws-ecs /> AWS EC2
  - VMs
    - <logos-aws-ec2 /> AWS EC2

<!--
  DEPLOYING
-->

---
image: https://source.unsplash.com/collection/1134422/1920x1080
level: 2
---

# Code Deployment

- CI/CD
  - Automated testing
  - Build And Deploy

<img v-click="[1,2]" src="/images/cd_1.png" class="h-80 absolute" />
<img v-click="[2,3]" src="/images/cd_2.png" class="h-80 absolute" />
<img v-click="[3,4]" src="/images/cd_3.png" class="h-80 absolute" />
<img v-click="[4,5]" src="/images/cd_4.png" class="h-80 absolute" />
<img v-click="[5,6]" src="/images/cd_5.png" class="h-80 absolute" />
<img v-click="6" src="/images/cd_6.png" class="h-80 absolute" />

<!--
  DEPLOYING
-->
---
layout: cover
background: ./images/entrance_3.jpg
level: 3
---

# **DEMO**

---
layout: cover
background: ./images/entrance_3.jpg
level: 2
---

# **THANK YOU**

<!--
  THANK YOU ALL
-->

---
layout: center
class: text-center
---

# Q&A

[LinkedIn <devicon-linkedin />](https://linkedin.com) · [Slides <carbon-logo-github />](https://github.com/interactivelabs/itz-presentation-2023)
