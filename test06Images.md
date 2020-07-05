#### Test Instructions
If the image is meaningful:
1.  Check that the combination of the accessible name and accessible description is not empty.
1.  Check that the non-empty combination of accessible name and accessible description provides an equivalent description. Numerous attributes contribute to the computation of the accessible name and accessible description. Refer to [HTML Accessibility API Mappings 1.0 for img](https://www.w3.org/TR/html-aam-1.0/#img-element).
    1.  Descriptions of the image that are provided by page content must be programmatically associated.
2.  Check that the ARIA role is NOT "presentation".
3.  Check that the ARIA role is NOT "none".
4.  Check that aria-hidden is NOT set to "true".
#### Test Results
-   If any of the above checks fail, then SC 1.1.1, SC 4.1.2, and Baseline Requirement 6 fail.
### Decorative Images
#### Test Instructions
If the image is decorative, check that at least one of the following is true:
1.  The ARIA role is "presentation".
2.  The ARIA role is "none".
3.  The aria-hidden state/value is set to "true".
4.  The combination of accessible name and accessible description is empty (e.g. ""). Numerous attributes contribute to the computation of the accessible name and accessible description. Refer to [HTML Accessibility API Mappings 1.0 for img](https://www.w3.org/TR/html-aam-1.0/#img-element).
5.  The image is inserted via CSS (e.g., using a background image).
#### Test Results
-   If all of the above checks fail, then SC 1.1.1, SC 4.1.2, and Baseline Requirement 6 fail.
### CAPTCHA Images
#### Test Instructions
If the Image is a Captcha image:
1.  Check that the combination of the accessible name and accessible description is not empty.
1.  Check that the non-empty combination of accessible name and accessible description identify and describe the purpose of the CAPTCHA.
2.  Check that alternative forms of CAPTCHA are provided, at a minimum, for users without vision and users without hearing.

#### Test Results
-   If any of the above checks fail, then SC 1.1.1, SC 4.1.2, and Baseline Requirement 6 fail.
Test Procedures for SC 1.4.5 Images of Text
-------------------------------------------
### Identify Content
Identify any images of text, except where a particular presentation of text is essential to the information being conveyed (e.g., logotypes or text that is part of a logo or brand name).
### Test Instructions
1.  Check that using text cannot achieve the same visual presentation and effect as images of text.
2.  Check that the image of text can be visually customized to a user's requirements.
    -   For example, web content allows users to specify font, size, color, and background settings, and all images of text are then provided based on those settings.
### Test Results
-   If any of the above checks fail, then SC 1.4.5 and Baseline Requirement 6 fail.
Advisory: Tips for streamlined test processes
---------------------------------------------
### WCAG 2.0 Techniques
-   The following sufficient techniques and/or common failures were considered when developing this test procedure for this baseline requirement:
    -   [ARIA6: Using aria-label to provide labels for objects](https://www.w3.org/TR/WCAG20-TECHS/ARIA6.html)
    -   [ARIA15: Using aria-describedby to provide descriptions of images](https://www.w3.org/TR/WCAG20-TECHS/ARIA15.html)
    -   [H36: Using alt attributes on images used as submit buttons](https://www.w3.org/TR/WCAG20-TECHS/H36.html)
    -   [H37: Using alt attributes on img elements](https://www.w3.org/TR/WCAG20-TECHS/H37.html)
    -   [H67: Using null alt text and no title attribute on img elements for images that AT should ignore](https://www.w3.org/TR/WCAG20-TECHS/H67.html)
    -   [G143: Providing a text alternative that describes the purpose of the CAPTCHA](https://www.w3.org/TR/WCAG20-TECHS/G143.html)
    -   [G144: Ensuring that the Web Page contains another CAPTCHA serving the same purpose using a different modality](https://www.w3.org/TR/WCAG20-TECHS/G144.html)
    -   [H86: Providing text alternatives for ASCII art, emoticons, and leetspeak](https://www.w3.org/TR/WCAG20-TECHS/H86.html)
    -   [F30: Failure of Success Criterion 1.1.1 due to using text alternatives that are not alternatives (e.g., filenames or placeholder text)](https://www.w3.org/TR/WCAG20-TECHS/F30.html)
    -   [F38: Failure of Success Criterion 1.1.1 due to not marking up decorative images in HTML in a way that allows assistive technology to ignore them](https://www.w3.org/TR/WCAG20-TECHS/F38.html)
    -   [F39: Failure of Success Criterion 1.1.1 due to providing a text alternative that is not null (e.g., alt="spacer" or alt="image") for images that should be ignored by assistive technology](https://www.w3.org/TR/WCAG20-TECHS/F39.html)
    -   [F65: Failure of Success Criterion 1.1.1 due to omitting the alt attribute or text alternative on img elements, area elements, and input elements of type = "image"](https://www.w3.org/TR/WCAG20-TECHS/F65.html)
    -   [C9: Using CSS to include decorative images](http://www.w3.org/TR/WCAG20-TECHS/C9.html)
----------------------------------------
[Home/Table of Contents](index.md) | [Previous Baseline](05Changing.md) | [Next Baseline](07Sensory.md)