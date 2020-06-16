## 508 Disability Compliance and Guidance

### Overall Guidance Notes
 Gvernment project, must accommodate all 508 disability requirements as required by federal law. In order to accommodate, some general purpose guidelines will be defined, and must be tested for release as part of the program lifecycle.

#### Section 508 Refresh
The US Access Board is in the process of updating the Section 508 requirements and, according to estimates, should be finalizing the new requirements at the end of 2015. Once the changes come into effect, the US Access Board will require compliance with the World Wide Web Consortium (W3C) Web Content Accessibility Guidelines (WCAG) 2.0 rather than trying to maintain their own unique set of standards. WCAG 2.0 Level AA will be the minimum to comply with Section 508 once the new standards come into effect.

####ARIA
W3C has also created a development language supplement called Web Accessibility Initiative (WAI) Accessible Rich Internet Applications (ARIA) Suite. It helps to identify and describe elements and how they relate to each other. This is a framework for adding attributes to complex applications that would otherwise be inaccessible because the native development language doesn't have certain capabilities. This enables technologies that have been inaccessible in the past to communicate more effectively with screen readers and other assistive technology devices. However, you don't need to double up. For example, if you are using an ```<h1>``` tag, there is no need to use ARIA to define the object's role as "heading". ARIA is only a supplement to help if a development language can't support identifying or describing elements in the application.

### Reference Material
####Current Section 508
1. U.S. Government page on [federal 508 disability compliance requirements](https://www.section508.gov/)
2. Section 508 [reference manual](https://www.section508.gov/archive-section508-reference)
3. U.S. General Service Administration (GSA) [Guidance for Software Applications and Operating Systems](http://www.gsa.gov/graphics/staffoffices/508softwareandos.doc)

####WCAG 2.0 (Section 508 Refresh)
4. [Web Content Accessibility Guidelines (WCAG) Overview](http://www.w3.org/WAI/intro/wcag "Web Content Accessibility Guidelines Overview")
5. [WCAG 2.0 Checklist](http://www.w3.org/TR/2006/WD-WCAG20-20060427/appendixB.html "WCAG 2.0 Checklist")
6. [How to Meet WCAG 2.0](http://www.w3.org/WAI/WCAG20/quickref/ "How to Meet WCAG 2.0")

####ARIA
7. [What is WAI-ARIA, what does it do for me, and what not?](http://www.marcozehe.de/2014/03/27/what-is-wai-aria-what-does-it-do-for-me-and-what-not/ "What is WAI-ARIA, what does it do for me, and what not?")
8. [Mozilla Developer Network – ARIA resource area](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA "Mozilla Developer Network – ARIA resource area")
9. [Accessible Rich Internet Applications (WAI-ARIA) 1.0 Standards](http://www.w3.org/WAI/PF/aria/ "	Accessible Rich Internet Applications 1.0")

### EPA Software Checklist (found as a reference [here](http://www.epa.gov/inter508/toolkit/508_compliance_toolkit_web_apps.htm))

1. Can you use the keyboard instead of the mouse? Use the keyboard exclusively to navigate through web pages & applications (particularly the tab and enter keys). Are all areas of the screen accessible? Are there keystrokes available for all mouse actions? Are there a minimum number of keystrokes to get to desired areas? Can you execute an action using the enter key without using a mouse?

2. Does the cursor move in a logical order or flow? Use the tab key to check where the cursor moves from one element to the next. The cursor should follow a logical order and not be random, e.g., the cursor should move top to bottom, left to right, or flow according to content.
Do the elements do what they are supposed to do? Use the return key after selecting a link or control element (e.g., radio buttons, boxes) to check for the appropriate action. For example, if you select a link, using the return key the link is opened; selecting a folder, opens the folder, etc.

3. Is there ALT text for all non-text elements? Check non-text elements (images, buttons, etc.) for appropriate alt (alternative) text. Alt text is needed when the image provides context or information or links to other areas. Alt text does not need to be provided for images that are for pure decoration, but does require the proper html code (ALT=""). Using this html code (ALT="") will tell the software not to read the graphic and will help the screen reader user. If you are familiar with code, you can look at the html code to check for alt text. If you are not a coder, place the mouse over the graphic or element and check for a box that appears with the text, similar to caption boxes.

4. Does the link text explain what the link "does"? Make sure that links make sense out of context. Avoid the use of "click here" and other vague instructions for links. Ex. Instead of "Click here" for a report use "Read the Report". People who use screen readers typically listen to all the links first to make sure they want to use the page. "Click Here" provides no context.

5. Are there captions for audio and visual elements or transcripts for audio only elements? If there is audio/visual multimedia, look for an indication that there are captions (symbol "CC", word "captions" or "text", etc.). How does the user know that there are captions? Do the captions work? Can you turn them on? Are the captions synchronized with the audio/visual elements? If it is audio only (ex. a radio broadcast or a podcast), look for a transcript (words such as "text", "transcript", "transcription", "script").

6. Is color the only means of identification of elements on a page? When colors are the only way to identify elements or controls on the screen, persons who are color blind, blind, or have low vision may find the web page unusable. Ex. a web page that directs a user to "press the red button to stop" should also identify the red button in another way than simply by color. To test for color: view the page on a black and white monitor, or print the page out on a black and white printer. Both methods will show if the removal of color affects the usability of the page.

7. Are documents organized so they are readable without requiring an associated style sheet? Since a style sheet is not required to create basic Web pages, you can just avoid style sheets entirely. But in cases where a style sheet is used, the Web page must be organized so that the information can still be accessed even for browsers that cannot use style sheets. When web developers set up their pages to override user-defined style sheets, people with disabilities may not be able to use those pages. It is critical that designers ensure that their web pages do not interfere with user-defined style sheets. You can avoid using style sheets altogether or you can use "external" style sheets, in which the style rules are set up in a separate file.

8. Are there server-side image map or client-side image maps? An "image map" is a picture (often an actual map) on a web page that provides different "links" to other web pages, depending on where a user clicks on the image. There are two basic types of image maps: "client-side image maps" and "server-side image maps." With client-side image maps, each "active region" in a picture can be assigned its own "link" (called a URL or "Uniform Resource Locator") that specifies what web page to retrieve when a portion of the picture is selected. If the web page uses a server-side image map to present the user with a selection of options, then a redundant text link is necessary to provide access to the page for anyone not able to see or accurately click on the map. FYI, at EPA you must use the standard US and regional maps and associated code for displaying information and to link to local information when applicable. The standard maps have the accessibility requirements taken care of for you. The EPA standard for maps of the US is available at http://yosemite.epa.gov/OEI/webguide.nsf/standards-guidance/maps2. If you create other maps, you will need to address this 508 standard.

9. Are tables coded properly? Tables are permitted, but 508 requires that tables be coded according to the rules of the markup language being used for creating tables. Large tables of data can be difficult to interpret if a person is using a non-visual means of accessing the web. Users of screen readers can easily get "lost" inside a table because it may be impossible to associate a particular cell that a screen reader is reading with the corresponding column headings and row names. The 508 standards apply to tables that have two or more logical levels of row or column headers. For more assistance, refer to US Access Board's guidance for tables.

10. Does your Web site have frames? Frames are not allowed at EPA. Do not use them. For more information, refer to the EPA Standard on Frames

11. Does the screen flicker with a frequency greater than 2 Hz and lower than 55 Hz? Some individuals with photosensitive epilepsy can have a seizure triggered by displays, presentations, backgrounds, and images that flicker, flash, blink, or rapidly change from light to dark within the range above. Do not use visuals that produce any vivid light-dark differences that change or flash between these rates. If your Web site is generally the same color or brightness without lots of rapid changes, then screen flickering is probably not a concern.

12. Are there text-only pages for information that cannot be made compliant in any other way? A text-only page, with equivalent information or functionality, shall be provided to make a Web site comply with the 508 standards, when compliance cannot be accomplished in any other way. Caution: the content of the text-only page needs to be updated whenever the primary page changes. Ex. a graphic of an org chart, plus a text-only version of the same information.

13. Is the script language in a readable fashion for assistive technology users? Web page developers need to provide script information in a fashion that can be read by assistive technology. When web developers do not put functional text with a script, a screen reader will often read the content of the script itself in a meaningless jumble of numbers and letters. Although this jumble is text, it cannot be interpreted or used. For more assistance, refer to US Access Board's guidance for scripts.

14. Is there a link for software downloads (Applets and Plug-ins)? Any page with information that requires extra software to be used such as Adobe, Word, Flash, etc. must also post a link to a free download of the software. FYI: in addition to 508 requirements, there are EPA web requirements for linking to PDFs - EPA PDF Links standard.

15. Are there electronic forms? For forms designed to be completed on-line, can people using assistive technology access the information, the form elements, and functionality so they can complete and submit the form? For more assistance, refer to US Access Board's guidance for electronic forms.

16. Is there a way for the user to skip navigation functions/sidebar and go straight to the content? Check skip navigation links to see if the next tab really bypasses the links and goes to the desired content. (*EPA Internet web pages using the EPA template already have this feature enabled. Internet pages that are not in the EPA template and Intranet pages need to address these standards)

17. If a timed-response is used, is the user prompted to request more time? Web pages, particularly data-entry pages, can be designed so that the page disappears or "expires" if a response is not received within a specified amount of time. If a timed-response is used, how does the user know that time is running out? How does a user indicate that more time is needed when they are prompted that time is starting to run out? This is not a common feature on EPA web pages
