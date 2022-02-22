
![DATE IRL Logo](/assets/images/DateIRL-V2.png)

This website was created to give singletons an outlet to connect with people in the real world. Without relying on dating apps.

## User Story

Joe is an ordinary guy. He has been split with his ex for 2 years now. And in the last year alone, he has been on 23 first dates. He has had 4 second dates and only 1 third date. But he has never made a lasting connection. Joe puts this down to the fact that he is only able to connect with people on a cosmetic basis. He sees them on the apps, swipes because he's attracted to them. And when they swipe back, a conversaation ensues via text message.

Joe likes this approach, overall, but he finds that when he meets the people in person, they tend to not look like their pictures, or they're not who they made themselves out to be during the text exchange. 

This why we created DateIRL. The text message barrier is broken down and we bring people together in a communal environment. People can be free to be themselves so that if there is a spark among singles, they can connect more naturally. Rather than wade through the potentials on an app.

## What We Built

The website is primarily an information portal for people who want to take part in a dating activity where they can connect with like-minded individuals with a view to finding a potential future partner.

The website consists of 4 pages which tell the user:

1. What we do and how it works
2. About us
3. A list of upcoming events
4. And a signup page to register interest

In the future, it is envisioned that the signup page will lead to a checkout, where users can actually reserve a spot, but for now, the information portal will suffice for the website's needs. Below are the initial wireframe models of the homepage on phone, tablet and desktop devices.


#### Mobile


![Date IRL - Mobile - Home](https://user-images.githubusercontent.com/99017752/154042180-7859a7b2-a686-4c2c-b366-4b4364e4b39b.png)


#### Tablet


![Date IRL - iPad - Home](https://user-images.githubusercontent.com/99017752/154042678-9765835f-6c45-4834-9180-7319a5036a81.png)


#### Desktop


![Date IRL - Desktop - Home](https://user-images.githubusercontent.com/99017752/154042744-dadc679f-563a-49a6-bf29-91f20b644571.png)


>It should be noted that the above is a base. The colour scheme and font are not cemented. These will be clarified later in the project.

## **22/2/2022**

### **Project re-direct**

Having met with mentor Ronan on Saturday 19/2, we determined that the website was currently looking very 90s Geocities/Angelfire style. There has been a change in the direction of the website. Now the project is taking a 2 page approach with 3 sections in the homepage. The pages as described above will still be present however, they will be sections of the homepage instead.

Below are some screenshots of the renderfed site in a locally developed version of VS Code.

**Mobile**

![DATE IRL Mobile](/assets/images/mobile.png)

**Tablet at 580px min-width**

![DATE IRL Mobile](/assets/images/min-width-580px.png)

**Desktop at 1170px min-width**

![DATE IRL Desktop at 1170px min-width](/assets/images/min-width-1170px.png)

The decision was taken to develop the site locally instead of in GitPod to prevent too many commits while the new site was being developed. Code will be copied over from local environment to GitPod. Will then run tests to confirm file paths are relevant and media queries remain as developed locally.

### **Testing**

Once all html code was finalised and CSS code was added, testing took the form of running media queries at various different screen-widths. It was determined that the 580px and 1170 screen widths were the optimal minimum widths for the content. The absolute position of the cover text element in the index.html was adjudged to not be detrimental to the UX of the website and no modification of same was required in terms of media queries.

Below is a screenshot from [AmIResponsive.com](http://ami.responsivedesign.is/) showing the various elements of the page at different screen widths.

![DATE IRL Responsiveness Test](/assets/images/responsiveness.png)

The next test was to check the Google Lighthouse report in Dev Tools

On first test, it displayed a poor performance score. 

![Lighthouse Test with no image optimisation](/assets/images/lighthouse-test-before-image-optimisation.png)

The presented opportunities indicated a high likelihood of performance imporvment with image optimasation, specifically in the events section of index.html and the sign-up.html file. 

![Opportunities presented by Lighthouse report](/assets/images/Opportunities.png)

As both elements used the same image, we optimised the image to reduce the overall image dimensions and also reduced the image quality slightly while still maintaining a render on the wenbsite which would be undetectable to the human eye. However,the LighthouseReport noticed it very well, when on running the report aafter image optimisation, it returned an almost perfecty performance score.

![Lighthouse Test after Image Optimisation](/assets/images/lighthouse-test-after-image-optimisation.png)

Lighthouse report aslo confirmed a high degree of accessibility achieving an overall score of 98%. Contrast is high and the only image elements are the logo areas in both pages. Any visible images are decorative backgroiund images with no `alt-text` required.

### **Validation**

On running the HTML files through the [Official W3C HTML Validation Tool](https://validator.w3.org/), itv was noticed that the section IDs were used in multiple instances. It was thought by this Junior Dev that IDs had some utility use cases, however this seems to not be case. These IDs were changed to classes where necessary, with specific references to the **Events** section of the index.html. This was also found in 1 instance in the `sign-up.html` file. The ID was modified here instead of changing to a class. The issue was in relation to a form label and input. So an ID was necessary in this case.

On re-running the HTML validator, no issues were found. The CSS validation was run after the HTML was updated and no issues were found in the [CSS Validation Tool](https://jigsaw.w3.org/css-validator/).

**index.html Validation**

![index.html Validation](/assets/images/index.html-validation-confirmation.png)

**sign-up.html Validation**

![sign-up.html Validation](/assets/images/sign-up.html-validation-confirmation.png)

**CSS Validation**

![CSS Validation](/assets/images/CSS-validation-confirmation.png)

### **Image Attribution**

**cool-backgroun.png** 

Gradient Topography SVG was provided by [https://coolbackgrounds.io/](https://coolbackgrounds.io/). The file was stored locally and a custom color scheme was applied by [NgenNo9](https://github.com/NgenNo9)

**glasses-clinking.jpeg**

Photo by Julia Kuzenkov from [Pexels](https://www.pexels.com/photo/people-having-a-toast-1974594/)

**DateIRL-V3**

Logo image designed by [NgenNo9](https://github.com/NgenNo9)

### **Deployment**

The site was deployed to a cloud-based platform. GitHub Pages provided the hosting of the deployment and can be viewed at [my project repo](https://ngenno9.github.io/project-1-DateIRL/).

### **Maintenance**

All files are stored locally within the repo so there is no need for maintenance as such. Justy to keep on top of the host to ensure it is fully operation and that teh website is being surfaced accordingly.