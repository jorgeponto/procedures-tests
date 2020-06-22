# Images

## Success Criteria applied to images (3)

- [SC 1.1.1 Non-text Content](sc111.md) - Level A
- [SC 1.4.5 Images of Text](sc145.md) - Level AA
- [SC 1.4.9 Images of Text (No Exception)](sc149.md) - Level AAA

## Procedures of techniques and failures applied to images (40)

- [ARIA6: Using aria-label to provide labels for objects](aria6.md)
- [ARIA9: Using aria-labelledby to concatenate a label from several text nodes](aria9.md)
- [ARIA10: Using aria-labelledby to provide a text alternative for non-text content](aria10.md)
- [ARIA15: Using aria-describedby to provide descriptions of images](aria15.md)
- [C9: Using CSS to include decorative images](c9.md[)
- [C22: Using CSS to control visual presentation of text](c22.md)
- [C30: Using CSS to replace text with images of text and providing user interface controls to switch](c30.md)
- [G68: Providing a short text alternative that describes the purpose of live audio-only and live video-only content](g68.md)
- [G73: Providing a long description in another location with a link to it that is immediately adjacent to the non-text content](g73.md)
- [G74: Providing a long description in text near the non-text content, with a reference to the location of the long description in the short description](g74.md)
- [G82: Providing a text alternative that identifies the purpose of the non-text content](g82.md)
- [G92: Providing long description for non-text content that serves the same purpose and presents the same information](g92.md)
- [G94: Providing short text alternative for non-text content that serves the same purpose and presents the same information as the non-text content](g94.md)
- [G95: Providing short text alternatives that provide a brief description of the non-text content](g95.md)
- [G100: Providing a short text alternative which is the accepted name or a descriptive name of the non-text content](g100.md)
- [G140: Separating information and structure from presentation to enable different presentations](g140.md)
- [G143: Providing a text alternative that describes the purpose of the CAPTCHA AND G144: Ensuring that the Web Page contains another CAPTCHA serving the same purpose using a different modality](g143.md)
- [G196: Using a text alternative on one item within a group of images that describes all items in the group](g196.md)
- [H2: Combining adjacent image and text links for the same resource](h2.md)
- [H24: Providing text alternatives for the area elements of image maps](h24.md)
- [H30: Providing link text that describes the purpose of a link for anchor elements](h30.md)
- [H35: Providing text alternatives on applet elements](h35.md)
- [H36: Using alt attributes on images used as submit buttons](h36.md)
- [H37: Using alt attributes on img elements](h37.md)
- [H44: Using label elements to associate text labels with form controls](h44.md)
- [H45: Using longdesc](h45.md)
- [H53: Using the body of the object element](h53.md)
- [H65: Using the title attribute to identify form controls when the label element cannot be used](h65.md)
- [H67: Using null alt text and no title attribute on img elements for images that AT should ignore](h67.md)
- [H86: Providing text alternatives for ASCII art, emoticons, and leetspeak](h86.md)
- [F3: Failure of Success Criterion 1.1.1 due to using CSS to include images that convey important information](f3.md)
- [F13: Failure of Success Criterion 1.1.1 and 1.4.1 due to having a text alternative that does not include information that is conveyed by color differences in the image](f13.md)
- [F20: Failure of Success Criterion 1.1.1 and 4.1.2 due to not updating text alternatives when changes to non-text content occur](f20.md)
- [F30: Failure of Success Criterion 1.1.1 and 1.2.1 due to using text alternatives that are not alternatives (e.g., filenames or placeholder text)](f30.md)
- [F38: Failure of Success Criterion 1.1.1 due to not marking up decorative images in HTML in a way that allows assistive technology to ignore them](f38.md)
- [F39: Failure of Success Criterion 1.1.1 due to providing a text alternative that is not null (e.g., alt="spacer" or alt="image") for images that should be ignored by assistive technology](f39.md)
- [F65: Failure of Success Criterion 1.1.1 due to omitting the alt attribute or text alternative on img elements, area elements, and input elements of type "image"](f65.md)
- [F67: Failure of Success Criterion 1.1.1 and 1.2.1 due to providing long descriptions for non-text content that does not serve the same purpose or does not present the same information](f67.md)
- [F71: Failure of Success Criterion 1.1.1 due to using text look-alikes to represent text without providing a text alternative](f71.md)
- [F72: Failure of Success Criterion 1.1.1 due to using ASCII art without providing a text alternative](f72.md)

## ACT-Rules

- [Image button has non-empty accessible name](https://act-rules.github.io/rules/59796f) - H36, G94, G95
  - **Applicability:** The rule applies to any HTML <code>input</code> element with a <code>type</code> attribute in the <a href="https://html.spec.whatwg.org/#image-button-state-(type=image)"><code>Image Button</code> state</a>, that is <a href="https://act-rules.github.io/rules/59796f#included-in-the-accessibility-tree" title="Definition of included in the accessibility tree">included in the accessibility tree</a>.
  - **Expectation:** Each target element has an <a href="#accessible-name" title="Definition of accessible name">accessible name</a> that is not empty (<code>""</code>). <strong>Note:</strong> Testing that the <a href="#accessible-name" title="Definition of accessible name">accessible name</a> describes the purpose of the element is not part of this rule and must be tested separately.
- [Image filename is accessible name for image](https://act-rules.github.io/rules/9eb3f6) - G94, G95, F30
  - **Applicability:** The rule applies to any HTML element with the <a href="https://act-rules.github.io/rules/9eb3f6#semantic-role" title="Definition of semantic role">semantic role</a> of <code>img</code> or any HTML <code>input</code> element with a <a href="https://html.spec.whatwg.org/#states-of-the-type-attribute"><code>type</code></a> of <code>image</code> when each of the following is true: (a) the image is <a href="https://act-rules.github.io/rules/9eb3f6#included-in-the-accessibility-tree" title="Definition of included in the accessibility tree">included in the accessibility tree</a>; and (b) the image has an <a href="https://act-rules.github.io/rules/9eb3f6#accessible-name" title="Definition of accessible name">accessible name</a> that is equivalent to the <a href="https://act-rules.github.io/rules/9eb3f6#filename" title="Definition of filename">filename</a> specified in the <code>src</code> attribute. Difference in letter casing, leading and trailing <a href="https://act-rules.github.io/rules/9eb3f6#whitespace" title="Definition of whitespace">whitespace</a> should be ignored.
  - **Expectation:** Each test target has an <a href="#accessible-name" title="Definition of accessible name">accessible name</a> that serves an equivalent purpose to the <a href="https://www.w3.org/TR/WCAG21/#dfn-non-text-content">non-text content</a>.
- [Image has non-empty accessible name](https://act-rules.github.io/rules/23a2a8) - G94, G95
  - **Aplicability:** The rule applies to HTML <code class="language-text">img</code> elements and HTML elements with the <a href="https://act-rules.github.io/rules/23a2a8#semantic-role" title="Definition of semantic role">semantic role</a> of <code class="language-text">img</code>, except for elements that are not <a href="https://act-rules.github.io/rules/23a2a8#included-in-the-accessibility-tree" title="Definition of included in the accessibility tree">included in the accessibility tree</a>.
  - **Expectation:** Each target element has an <a href="https://act-rules.github.io/rules/23a2a8#accessible-name" title="Definition of accessible name">accessible name</a> that is not empty (<code class="language-text">""</code>), or has a <a href="https://act-rules.github.io/rules/23a2a8#semantic-role" title="Definition of semantic role">semantic role</a> of <code class="language-text">none</code> or <code class="language-text">presentation</code>.
- [Image not in the accessibility tree is decorative](https://act-rules.github.io/rules/e88epe) - 
  - **Aplicability:** Any <code class="language-text">img</code>, <code class="language-text">canvas</code> or <code class="language-text">svg</code> element that is <a href="https://act-rules.github.io/rules/23a2a8#visible" title="Definition of Visible">visible</a> and for which one of the following is true:
    - <strong>excluded</strong>: The element is not <a href="https://act-rules.github.io/rules/23a2a8#included-in-the-accessibility-tree" title="Definition of Included in the accessibility tree">included in the accessibility tree</a>; or
    - <strong>ignored svg</strong>: The element is an <code class="language-text">svg</code> with an empty (<code class="language-text">""</code>) <a href="https://act-rules.github.io/rules/23a2a8#accessible-name" title="Definition of accessible name">accessible name</a> and a <a href="https://act-rules.github.io/rules/23a2a8#semantic-role" title="Definition of Semantic Role">semantic role</a> of <code class="language-text">graphics-document</code>; or
   - <strong>ignored canvas</strong>: The element is a <code class="language-text">canvas</code> with an empty (<code class="language-text">""</code>) <a href="https://act-rules.github.io/rules/23a2a8#accessible-name" title="Definition of accessible name">accessible name</a> and no <a href="https://act-rules.github.io/rules/23a2a8#explicit-role" title="Definition of Explicit semantic role">explicit semantic role</a>; or
   <strong>Exception</strong>: This rule never applies to elements for which one of the following is true:
   - The element has an <a href="https://dom.spec.whatwg.org/#concept-tree-ancestor" title="DOM definition of ancestor, 2020/03/06">ancestor</a> in the <a href="https://drafts.csswg.org/css-scoping/#flat-tree" title="CSS Scoping definition of Flat tree, working draft">flat tree</a> that is <a href="https://www.w3.org/TR/wai-aria-1.1/#namecalculation" title="WAI-ARIA definition of Named from author">named from author</a>; or
   - The element is an <code class="language-text">img</code> element where the <a href="https://html.spec.whatwg.org/#current-request" title="HTML definition of Current request, 2020/03/06">current request</a>'s <a href="https://html.spec.whatwg.org/#img-req-state" title="HTML definition of Image request state, 2020/03/06">state</a> is not <a href="https://html.spec.whatwg.org/#img-all" title="HTML definition of Completely available, 2020/03/06">completely available</a>. <strong>Note</strong>: An example of an image ignored because of an <a href="https://dom.spec.whatwg.org/#concept-tree-ancestor" title="DOM definition of ancestor, 2020/03/06">ancestor</a> with <a href="https://www.w3.org/TR/wai-aria-1.1/#namecalculation" title="WAI-ARIA definition of Named from author">named from author</a> is when the image is a descendant of a <code class="language-text">button</code> element that uses <code class="language-text">aria-label</code> for its accessible name.   
  - **Expectation:** Each test target is <a href="https://www.w3.org/TR/WCAG21/#dfn-pure-decoration" title="WCAG definition of Pure decoration">purely decorative</a>. <strong>Note</strong>: It is relatively common for an informative image such as an icon to be marked up as decorative, if the text alternative is adjacent to the image. This is a <a href="https://www.w3.org/TR/WCAG21/#dfn-conforming-alternate-version" title="WCAG definition of Conforming alternative version">conforming alternative version</a> for the image. This fails the rule but meets <a href="https://www.w3.org/TR/WCAG21/#cc1">conformance requirement 1 of WCAG 2.1</a>.

- [svg element with explicit role has non-empty accessible name](https://act-rules.github.io/rules/7d6734)
  - **Aplicability:** The rule applies to any element in the <a href="https://www.w3.org/2000/svg">SVG</a> namespace with an <a href="https://act-rules.github.io/rules/7d6734#explicit-role" title="Definition of explicit role">explicit semantic role</a> of either <code class="language-text">img</code>, <code class="language-text">graphics-document</code>, <code class="language-text">graphics-symbol</code>, that is <a href="https://act-rules.github.io/rules/7d6734#included-in-the-accessibility-tree" title="Definition of Included in the accessibility tree">included in the accessibility tree</a>.
  - **Expectation:** Each target element has an <a href="https://act-rules.github.io/rules/7d6734#accessible-name" title="Definition of accessible name">accessible name</a> that is not empty.

## Map of Test Procedures (97 tests = 40+32+18+5+1+1)

| TechniK |     |     |     |     |     |     |
| ------- | :-: | :-: | :-: | :-: | :-: | :-: |
| [ARIA6](aria6.md) | [1](aria6.md#n1 "ARIA6") ||||||
| [ARIA9](aria9.md) | [1](aria9.md#n1 "ARIA9") | [2](aria9.md#n2 "ARIA9") |||||
| [ARIA10](aria10.md) | [1](aria10.md#n1 "ARIA10") | [2](aria10.md#n2 "ARIA10") | [3](aria10.md#n3 "ARIA10") ||||
| [ARIA15](aria15.md) | [1](aria15.md#n1 "ARIA15") | [2](aria15.md#n2 "ARIA15") | [3](aria15.md#n3 "ARIA15") ||||
| [C9](c9.md) | [1](c9.md#n1 "C9") | [2](c9.md#n2 "C9") |||||
| [C22](c22.md) | [1](c22.md#n1 "C22") ||||||
| [C30](c30.md) | [1](c30.md#n1 "C30") | [2](c30.md#n2 "C30") |||||
| [G68](g68.md) | [1](g68.md#n1 "G68") | [2](g68.md#n2 "G68") | [3](g68.md#n3 "G68") ||||
| [G73](g73.md) | [1](g73.md#n1 "G73") | [2](g73.md#n2 "G73") | [3](g73.md#n3 "G73") | [4](g73.md#n4 "G73") |||
| [G74](g74.md) | [1](g74.md#n1 "G74") | [2](g74.md#n2 "G74") | [3](g74.md#n3 "G74") ||||
| [G82](g82.md) | [1](g82.md#n1 "G82") | [2](g82.md#n2 "G82") | [3](g82.md#n3 "G82") ||||
| [G92](g92.md) | [1](g92.md#n1 "G92") | [2](g92.md#n2 "G92") | [3](g92.md#n3 "G92") ||||
| [G94](g94.md) | [1](g94.md#n1 "G94") | [2](g94.md#n2 "G94") | [3](g94.md#n3 "G94") | [4](g94.md#n4 "G94") |||
| [G95](g95.md) | [1](g95.md#n1 "G95") ||||||
| [G100](g100.md) | [1](g100.md#n1 "G100") | [2](g100.md#n2 "G100") |||||
| [G140](g140.md) | [1](g140.md#n1 "G140") | [2](g140.md#n2 "G140") |||||
| [G143](g143.md) | [1](g143.md#n1 "G143") | [2](g143.md#n2 "G143") | [3](g143.md#n3 "G143") ||||
| [G196](g196.md) | [1](g196.md#n1 "G196") | [2](g196.md#n2 "G196") | [3](g196.md#n3 "G196") ||||
| [H2](h2.md) | [1](h2.md#n1 "H2") | [2](h2.md#n2 "H2") |||||
| [H24](h24.md) | [1](h24.md#n1 "H24") | [2](h24.md#n2 "H24") |||||
| [H30](h30.md) | [1](h30.md#n1 "H30") | [2](h30.md#n2 "H30") | [3](h30.md#n3 "H30") | [4](h30.md#n4 "H30") |||
| [H35](h35.md) | [1](h35.md#n1 "H35") | [2](h35.md#n2 "H35") | [3](h35.md#n3 "H35") ||||
| [H36](h36.md) | [1](h36.md#n1 "H36") | [2](h36.md#n2 "H36") |||||
| [H37](h37.md) | [1](h37.md#n1 "H37") | [2](h37.md#n2 "H37") | [3](h37.md#n3 "H37") ||||
| [H44](h44.md) | [1a](h44.md#n1a "H44") | [2a](h44.md#n2a "H44") | [3a](h44.md#n3a "H44") | [1b](h44.md#n1b "H44") | [2b](h44.md#n2b "H44") | [3b](h44.md#n3b "H44") |
| [H45](h45.md) | [1](h45.md#n1 "H45") | [2](h45.md#n2 "H45") | [3](h45.md#n3 "H45") ||||
| [H53](h53.md) | [1](h53.md#n1 "H53") ||||||
| [H65](h65.md) | [1](h65.md#n1 "H65") | [2](h65.md#n2 "H65") | [3](h65.md#n3 "H65") ||||
| [H67](h67.md) | [1](h67.md#n1 "H67") | [2](h67.md#n2 "H67") |||||
| [H86](h86.md) | [1](h86.md#n1 "H86") | [2](h86.md#n2 "H86") |||||
| [F3](f3.md) | [1](f3.md#n1 "F3") | [2](f3.md#n2 "F3") | [3](f3.md#n3 "F3") ||||
| [F13](f13.md) | [1](f13.md#n1 "F13") ||||||
| [F20](f20.md) | [1](f20.md#n1 "F20") ||||||
| [F30](f30.md) | [1](f30.md#n1 "F30") ||||||
| [F38](f38.md) | [1](f38.md#n1 "F38") | [2](f38.md#n2 "F38") |||||
| [F39](f39.md) | [1](f39.md#n1 "F39") | [2](f39.md#n2 "F39") |||||
| [F65](f65.md) | [1](f65.md#n1 "F65") | [2](f65.md#n2 "F65") | [3](f65.md#n3 "F65") | [4](f65.md#n4 "F65") |||
| [F67](f67.md) | [1](f67.md#n1 "F67") ||||||
| [F71](f71.md) | [1](f71.md#n1 "F71") | [2](f71.md#n2 "F71") |||||
| [F72](f72.md) | [1](f72.md#n1 "F72") | [2](f72.md#n2 "F72") |||||
