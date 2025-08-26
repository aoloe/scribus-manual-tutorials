# Scribus Tutorials Review

A list of good tutorials for Scribus.

## Video introductions

### Tj's Scribus Lessons

- [Scribus Lesson 1 - Getting Started and User Interface](https://www.youtube.com/watch?v=hMlT9C6xcDw)
  - Shows the development version
  - Negative points:
    - Creates two columns without using guides.
    - Resizes the picture frame, instead of scaling the picture to the frame.
    - Shows exporting to images (only PDF should be presented to beginners).
  - Remarks:
    - Outside of the "imperial" world, you should use "mm" as the unit.
- [Scribus Lesson 2- Image Frames and Properties](https://www.youtube.com/watch?v=nB4dTL1IwI4)
  - Negative points:
    - Moving the image in the frame is not a beginner's task. The image should fit the frame and the frame fit to it. Then move around the frame.
    - Should not show editing the frame name
    - At the end of the tutorial, the two frames are not nicely aligned to anything.
  - Remarks:
    - Using the Properties Palette, Image tab, is a better way to fit the image in the frame.
    - Should dock the Properties palette to the right side.
- [Scribus Lesson 3- Add Text Frames](https://www.youtube.com/watch?v=JTo_NZeOPqA)
  - Errors:
    - Don't show the story editor for editing (long) text. It's only for special case (inverted text, ...)
  - Remarks:
    - He should first show making a frame longer when the text overflows, than chaining with the next frame.
    - Should really use guides
    - Should first show the sample text, than typing...
- [Scribus Lesson 4 - Add & Remove Pages](https://www.youtube.com/watch?v=INVeoAx8J-g)
- [Scribus Lesson 5 - Using Templates](https://www.youtube.com/watch?v=N0_3XnraPQI)
- [Scribus Lesson 6 - Numbering Pages](https://www.youtube.com/watch?v=f-228vBWOSI)
- [Scribus Lesson 7 - Master Pages](https://www.youtube.com/watch?v=tEiJlyuVndY)
- [Scribus Lesson 8 - Using Syles](https://www.youtube.com/watch?v=rkyX7rgeawg)
- [Scribus Lesson 9 - Colors & Color Management](https://www.youtube.com/watch?v=Eaemh2DOQZk)
- [Scribus Lesson 10 - Flow Text Around Image Frame](https://www.youtube.com/watch?v=DXrabr1FYegi)

### Graphic design for Free

[Scribus, the free and professional page layout program for Windows, Mac, and Linux](https://www.youtube.com/watch?v=PBHh8aUB34s&list=PLHl8nuacOfLK709_hb3ViX3Nef9WchSQH)

General comments:

- 👍 Many small videos about specific topics
- 👍 It presents the tutorials series as covering the development version of Scribus, but since it's a few years old, it actually mostly covers the current stable version.
- 👍 Presents many real world _advanced_ issues and how to solve them with Scribus (sometimes with _hacks_ sometimes with Scribus features).
- 👍 Very visually pleasant examples, close to what a good graphic designer would create. Most of the time they are also easy to replicate.
- 👎 If you're looking for a solution for a specific issue, it might be there, but it's not easy to find out which clip covers them (example: creating a typographic correct 1/6 fraction is presented in _Superscript and subscript_).
- 👎 Presents features (transparencies...) that are often not supported by print houses: should give a big warning that Scribus does not flatten transparencies and, on the other side, print houses often ask for _modern_ PDF version but explicitly or implicetly require the transparencies to be flattened.
- 👎 Does not go into typical issues that you can encounter when sending Scribus PDFs to print houses: often they know how to work around Indesign shortcomings, but will just blame Scribus, if their workflow does not conform to the standards they're requiring.

✎ = edits, corrections, addendums
⚙ = Remarks for the developers

Review of the chapters:

- 0. Scribus, the free and professional page layout program for Windows, Mac, and Linux
  - Some nice visuals.
  - No real content
  - ✎ A few visuals have notting to do with Scribus.

#### Getting Scribus

- 1. Install Ghostscript for Scribus
  - ✎ Most people do not need Ghostscript: it should not be one of the first chapters.
  - Correctly says where you can get Ghostscript and how to configure Scribus to use the installed Ghostscript.
  - ✎ Does not say for what you need Ghostscript:
    - Render frames (Latex).
    - Loading a PDF into an image frame.
    - Loading an EPS (vector and bitmap) into an image frame.
  - ✎ Some wrong (outdated) information:
    - You don't need Ghostscript to import PDFs into Scribus.
    - The preview (nor the color separation preview) does not use Ghostscript but is PDF based.
- 2. Installing Scribus
  - Correctly shows how to get to the Scribus download links
  - ✎ The development version shown in the tutorials is very similar to the current stable version 1.6.
  - ✎ Should tell how to choose between stable and devlopemnt version:
    - Correctly names it development and not unstable.
    - In most cases, using the development version is indeed fine.
    - Beginners should start with a stable version and only move to a development version if:
      - They are comfortable with it.
      - Know what are its drawbacks (there are features that are there but should not be used...)
      - Need some new features or want to profit from an improved UI.
  - ✎ Only tells how to install on Windows
    - MacOs is roughly the same, but you need to take care about the different platforms.
    - On Linux you should prefer installing from your distribution's package; If it's not available (in a current / desired version), you can install the Appimage.

#### Setting up Scribus

- 3. Preferences in Scribus
  - Setting the colors in the Scribus canvas
  - ✎ You can also change the colors of the guides and margins while a document is open, but the changes (as always for the prerefences), will apply to the document you will open in the future.
  - ✎ You can also change the guides / margins colors for a specific document, by using the same section and tab in the _Document Setup_ (but you can't use ad hoc values for the other colors).
  - ✎ Should better explain that changes in the preferences apply in two ways:
    - _Global_ preferences generally apply to how Scribus behaves (like the colors in the _Preferences > Display_ section.
    - _Document_ preferences apply to the document you will be creating in the future (you can recognize them by the fact that the same properties are also in the _Document Setup_ dialog.
- 4. Customizing the Scribus user interface
  - ✎ If your vertical screen estate is smaller than what shown in the video, you should probably hide the _other_ toolbars (and only keep the _Tools_ tolbar vertically docked as shown in the video.
  - ✎ Should show how to enable / disable a toolbar (context menu on the toolbar itself).
  - ✎ If you really think that you need the _File_ and _Edit_ toolbars, you should keep it as an horizontal toolbar.
  - ✎ You only need the _PDF Tools_ toolbar while you are editing a PDF form. You can keep it hidden most of the time.
  - ✎ Sadly, The _View Tools_ toolbar is just badly done and mixes features that most people never use (preview quality, visual appearance), feature that you might use (enabling the editing in the preview mode), and other that you should better use with a keyboard shoertcut (entering and exiting the preview mode: ctrl-alt-p)
  - ✎ Should better present _Tools_ toolbar, the content and properties palettes as the main UI elements in Scribus (Scribus has four main _concepts_: the Canvas, the _Tools_ toolbar, the Properties and Content Palettes, the _Preferences_ and the _Document Setup_: They should be presented in their own chapter before the customization step).
  - ✎ The _Properties_ and _Content_ palette might be shown also as tabs, switching between them with F2 and F3.

#### First steps with Scribus

- 5. Create a new document in Scribus
  - Introduction to units.
  - Introduction to the page size.
  - Introduction to margins and bleeds.
  - ⚙ TODO: does it mention somewhere how to add other (and custom) page sizes?
- 6. Image Frame and resolution
  - Introduction to zooming.
  - Introduction to image resolution.
  - ✎ Should say that Scribus uses the "Image resolution" value shown below the preview in the _Load Image_ dialog.  
    The value of the preview is set by the image editor (for Gimp: _Image > Print Size_; this is not the same as scaling the image: the number of pixel does not change).  
    In the given video you see that the first image has 300 dpi, the second one 72 dpi: the values are reflected in the _Load Image_ dialog and in the property palette.
  - ✎ Should mention that the required resolution depends on the paper, the printing technology and from the type of document (distance of viewing / reading)
  - ✎ Should mention that there is a minimal resolution and a target resolution for printing.
  - ✎ Misses the chance to warn that if the image at its current resolution is much bigger than the frame, you might only see its top left corner: if that is all white, you might think that the imge is not loaed at all.
  - ✎ 300 dpi is not a minimum for an image to print: it's not a bad default but, depending on the printing technology, you might not need that much resolution (newpsaper, some magazines) or might need much more (photo book)
- 7. Image frame options in Scribus
  - Second introduction to DPI.
  - Shows how to set the minimum resolution for images in the _Preflight verifier_ preferences.
  - Cropping images in the frame and moving them inside of the frame.
  - ✎ Should warn that the whole images is always included in the exported PDF (no real cropping)
- 8. Adjust and create image frames in Scribus
  - Presenting the nodes editor.
  - ✎ When creating a circular frame:
    - If it's a one time thing, it's better to create a regular image frame and modify its shape in the _Shape_ tab of the _Properties palette_
    - But it's useful to learn that you can convert items into other types of frames.
  - ✎ Should import a better shape from Inkscape.
  - How to remove the border in a shape / frame.
  - ✎ Should explain the difference between borders that will be printed and the frame _decorations_ in the UI.
  - ✎ Should introduce the shortcut for the preview mode (ctrl-alt-p) and the fact that in preview mode the document cannot be modified.
  - Introduces ctrl-alt for scaling the content proportionally.
- 9. Importing images with layers in Scribus
  - How to create images with layers in Gimp and how to work with them in Scribus.
  - ✎ It might be a bit early for presenting these advanced image properties, but it's well done (it's the longes tutorial up to now, and it's mostly about Gimp).
  - ✎ Should explain why PSD is chosen as the image format.
  - ✎ The image frame tool can be activated with the key _i_
  - ✎ When an image frame is selected, ctrl-i start the loading of an image.
- 10. Import images with transparency in Scribus
  - How to add transparency in Gimp and how to do it with clipping paths.
  - ✎ It might be a bit early for presenting these advanced image properties, but it's well done (it's the longes tutorial up to now, and it's mostly about Gimp).
  - ✎ Should explain why TIF and PNG are chosen as the image format for clipping path and alpha channel.
- 11. PDF version and transparency
  - Explains why a transparency created with alpha channel is risky for printing and why a clipping path is the better solution
  - ✎ Should warn that even if the PDF version allows transparencies, the printing house might still not respect and ignore the transparency information.
- 12. Make text flow around images in Scribus
  - ✎ It should first introduce text frames...
  - Adding a padding around _floating_ images and edit / use the contour line.
  - Examples for shapes, for images with transparencies and for images with a path.
  - ⚙  TODO: Scribus 1.7, should get a simpler way to add a padding around images

#### Formatting text

- 13. Text frames in Scribus
  - Create a text frame
  - Fill the text frame with sample text.
  - Move and rotate the frame, moving the the frame shape without rotating the text.
  - Create frames of different shapes.
  - Forced justification.
  - Line spacing: fixed, automatic.
  - Importing text from a word document (with or without formatting).
  - ✎ The text frame tool can be activated with the key _t_
- 14. Paragraph Styles in Scribus
  - Every text has a default style.
  - ⚙ TODO: the author suggest to highlight in the UI when local formatting is applied (without using a style).
  - Showing the control characters.
  - Editing a paragraph style and creating a new one.
- 15. Character styles in Scribus
  - Creating and applying character styles.
- 16. Hard Return vs Soft Return in Scribus
  - Return and shift-return.
  - ✎ Using shift return for a new line without a paragraph break is not always a good idea: if your text is justified then the lines with a shift-return will be forced justified
  - ✎ Having a space below the paragraph that is not a multiple of the line spacing will give uneven lines in multicolumn text.
- 17. Using Tabs in Scribus: left, right, period, comma, and centered
  - One shall create and move the tabs in all affected paragraphs at once.
  - Normally, tabs sould be defined in paragraph styles.
- 18. Hanging Indents in Scribus
  - Define a paragraph style with hanging indents for a list of items.
- 19. Drop Caps in Scribus
- 20. Paragraph Spacing and Indenting in Scribus
  - ✎ The space below the paragraph should be a multiple of the line height.
- 21. Cloning a Paragraph Style in Scribus
  - Duplicating a styles and modifying specific formatting.
  - ✎ Seems to be a step towards style inheritance in the next chapter
- 22. Style inheritance in Scribus
  - Creating _substyles_ (extending a style with specific formatting)
  - ✎ It should probably be the other way round: The _Drop caps_ style should be a child of the _Body text_ one.
- 23. Dot leaders in Scribus
  - More information about style inheritance, using a manual table of contents for the example.
  - Sytematic creation of character and paragraph styles for a table of contents.
  - More on adding tabs and using a tab leader.
- 24. Inline Objects in Scribus
  - Adding an image that should flow with the text.
  - Resizing / editing inline items.
  - Reusing the same inline item (for fancy list bullets)
  - ✎ Don't use it too much for images: it does not work as good as most user would want it to work.
- 25. Glyphs, Ligatures and Typographer's Quotes in Scribus
  - In text edit mode, _Insert > Glyph_
  - ✎ For typographic quotes, Scribus provide the script _Autoquote2_.
  - Manually insert ligatures that are not automatically applied

#### Page layout

- 26. Columns inside a text frame in Scribus
  - Create a text frame and define the number of columns and a gutter.
  - ✎ When the an _item_ tool is active, holding shift while clicking on the page, will will the page with the newly created frame (if there are guide on the page, the frame will extend to the next guide).
- 27. Create a three Column grid in Scribus
  - Using the column tab in the _Edit > Guides manager_

#### Vector graphics

- 28. Create Color swatches in Scribus
  - Choosing the default color set.
  - Adding a color
- 29. The Line tool in Scribus
  - Drawing a line and giving it a color.
  - ✎ Of course, it does not really make sense to use solid lines for having a different color for the guides: just change the color in the _Document Setup > Guides_.  
    But it's a nice trick for introducing layers...

#### Miscellanous topics

- 30. Working with Layers in Scribus
  - Create a new layer, moving the content to it, protecting them from editing.
  - Introducing the settings for the layers.
  - ✎ It might need a more meaningful use case for the layers.
  - ✎ _Enable selecting_ is in this case not a good idea (you don't really want to select the lines! But you don't really want lines instead of guide either).
  - ✎ Might want to warn that as soon as you have layers, you might activate the wrong layer and having the feeling that nothing can be edited anymore...
- 31. Linking Text Frames in Scribus
  - Creating columns and linking them
  - Resizing the columns
  - ✎ Using shift-click better fills the columns.
  - ✎ For better workflows:
    - shift-click the first column and keep it selected, activate the _Link text frame_ tool and shift-click in the second column, ...
    - shift-click the first column, fill it with more text than it can display, click on the overflow mark at the lower right corner of the frame and shift-click the second column to create a new column and let the text flow into it.
  - ✎ Might want to show a heading that spans the three columns
  - ✎ Might want to show a magazine page, with two articles, heading spanning multiple columns, images spanning multiple columns.
- 32. Smart guides in Scribus
  - _Page > Snap to items_
  - Introduction to the _Path tools_ for merging or diffing shapes.
  - ✎ Still, you probably should do more complex vector drawing in Inkscape.

#### Working on longer documents

- 33. The Baseline Grid in Scribus
  - Align text over multiple columns with the baseline grid.
  - Defining it in the _Document setup_ and applying it in the _Paragraph style_.
  - The text frame should be higher than the last line to avoid that the descenders give a column break.
- 34. Create new pages in Scribus
  - Copy the current page and (if you want it) link the last frame of a page to the first one in the next page.
  - ✎ Alternative: create enough empty pages and use _Edit > Multiple duplicate > By page_ to duplicate the current (empty) frames into the next pages and link them.
  - _Facing pages_ page layout.
  - Using the _Arrange pages_ palette.
  - Deleting pages.
- 35. Master pages in Scribus
  - Adding page numbering on the master page
  - Applying a specific master page to the left or right pages in the document.
    Could need a better example for the master pages.
- 36. Convert to Master page in Scribus
  - Putting the column margin lines in the master page.
  - ✎ The use case is a bit silly... Probably better to go directly for page numbers (first applied on the page, then moved to the master page).
- 37. Page Numbers in Scribus
  - Adding page numbers in the footer for facing pages.
  - Adding page numbers on a page with a solid background.
  - ✎ Better explain that the order of layers works accross master pages and pages: If the document has full page images (or shapes) that should be below the page numbers you can put the page number on a separate layer that is above the body content.
  - ✎ In page layout, you don't set the background color of the page, but add colored shapes behind all other items.
- 38. Adding Sections in Scribus
  - _Document Setup > Document Sections_
  - For defining the starting page number or its style.
- 39. Grid hierarchy in Scribus
  - Setting the visual order of the guides to be the same as in Indesign.
  - ✎ No need to close all documents to change the preferences for the future documents.
- 40. Page navigation and Bookmarks in Scribus
  - Bookmarks can be put outside of the page and used for navigating Scribus or also added to the PDF exported.

#### Working with items

- 41. Sticky Tools in Scribus
  - Sticky tools will keep the item tool selected after having used it (by default Scribus changes automatically to the _Move_ tool).
  - Finally presenting shift-click
  - ✎ Further optimisation: You don't even need to click on the overflow icon: just press the n key (for next frame) just after having created the text frame that fills the column and shift-click on the next column...
- 42. Selecting objects in Scribus
  - The _Outline_ tool
  - ctrl-key for cycling through the items below the cursor.
  - shift-click to select multiple items
  - use the Properties palette to move up and down the level of the item.
- 43. Grouping objects in Scribus
  - Selecting items in a group with the _Outline_ tool
  - ✎ alt-click also selects single items inside of a group (can be combined with ctrl and shift)
  - Using the _Align and distribute_
  - Editing text inside of a group
    - Selecting the text frame with the _Outline_ tool or alt-click.
    - Double click on the selected text frame (in the Outline tool or on canvas) or press the _e_ key while it's selected to start the edit mode.
  - Create a badge as a _complex_ group of shapes and text.

#### _Decorating_ your document

- 44. Color Gradients in Scribus
  - Use different type of gradients as the fill color of a shape.
  - ✎ Be aware that depending on the PDF version and the print house you might not correctly print the gradients.
  - Create a badge as a _complex_ group of shapes and text.
- 45. Transparency in Scribus
  - Adding a rectangle with 70% transparency to increase the readability of a text placed over an image.
  - Make text transparent
  - Make gradients fade to transparency
  - ✎ Be aware that depending on the PDF version and the print house you might not correctly print the transparency.
- 46. Transparency vs Blending modes in Scribus
  - The multiply blending mode
- 47. Blending modes in Scribus
  - Adding a pattern behind an image
  - ✎ Not sure that they can be correctly printed, indpendently of the PDF version and the print house requirements.
- 48. Non-Destructive Image Editing in Scribus
  - _Image effects_
  - ✎ Before using the effects, make sure with your print house, that they will correctly print them.
- 49. Duotone images in Scribus
  - Grayscale effect
  - Multiply blending mode with a colored rectangle.
  - ✎ Before using the effects, make sure with your print house, that they will correctly print them (most of all, if you want to have a control on the color plates used).
- 50. Scribus to Gimp Quick connect
  - Use Gimp as the external editor from Scribus

#### Text tweaking

- 51. Hyphenation and Justification in Scribus
  - _Extras > Hyphenate text_
  - Enable _Optical margins_.
  - Tweak the _Min. space width_ and the _Glyph extension_ in the paragraph style's _Advanced settings_ (or _Typography_ in 1.7+).
  - Inserting soft hyphens (ctrl--)
- 52. Kerning and Tracking in Scribus
  - Tracking: reduce the width of glphys on specific parts of the text.
  - Kerning: reduce the space between glphys on specific parts of the text.
- 53. Superscript and Subscript in Scribus
  - Creating a correct looking 1/6.

#### _Decorating_ your document

- 54. The Bezier Curve tool in Scribus
  - How to draw a Bezier curve.
  - Recommending to use Inkscape for complex vector graphics.
  - ✎ In 1.8 the nodes tool will be much improved (but still not as comfortable as in Indesign)
- 55. Place Text on a Path in Scribus
  - Create a path and attach text to it.
  - Tweak the text to look good.
  - Using the Story Editor to edit the text.
- 56. Mesh Distortion in Scribus
  - Using the Mesh distorition tool for _artistic_ graphic effects
  - Recommending to use Inkscape for complex vector graphics.
- 57. Align and Distribute in Scribus
  - Using the "Align and Distribute" tool for alignment.
  - Distributing items at equal gaps.
  - ✎ Depending on the task, _Align to items_ with ctrl-move (axis constraint) can also be a good solution.
- 58. The Eye Dropper in Scribus
  - Using the color picker to get a color from an image placed in Scribus
  - ✎ This method is not very exact.
- 59. Stroke and Fill in Scribus
  - Setting the default stroke and fill colors in the preferences.
  - Defining a line width.
  - ✎ Since the user cannot control the _direction_ of the line (inside the shape, on the border, outside of the shape), thick borders are a bit of a hit and miss.
- 60. Drop Shadow in Scribus
  - Adding a drop shadow to an image frame.
  - Adding a curved drop shadow.
  - ✎ Drop shadows are calculation intensive and might slow down SCribus.
  - ✎ Depending on the PDF version and the printing house requirements, drop shadows will not correctly print.
- 61. Rounding Endcaps and Corners in Scribus
- 62. Dashed & Dotted Lines in Scribus
  - Creating custom dashed patterns
  - Adjusting dashes for shape corners
  - Creating a dotted text outline.
- 63. Arrows in Scribus
  - Adding arrows to lines and beziers.
  - Creating a cut line with scissors arrow heads.

#### Text formatting

- 64. Inset Spacing and Vertical Centering in Scribus
- 65. Highlight text in Scribus
  - Background color in character styles.

#### Miscellanous topics

- 66. Stroke transparency in Scribus
  - ✎ Setting the opacity of the stroke or a line seems to be working. Is it really needed to use the layer transparency?
  - ✎ Depending on the PDF version and the printing house requirements, transparencies will not correctly print.
  - ✎ One can use _Send to layer_ in the context menu for sending an item from the current layer to a different one (no need to cut and paste).
- 67. Multiple Duplicate in Scribus
  - Duplicate with gaps or in columns and rows.
- 68. Fast Zooming in Scribus
  - ctrl-1 for _real size_.
  - ctrl-0 for fitting to height. 
  - ctrl-mouse wheel for zooming in and out (stepping can be set in the preferences)
- 69. Creating Shortcuts in Scribus
  - Loading custom Indesign shortctuts (by the author of the tutorials).
  - Defining custom shortcuts.
- 70. Column Break vs Frame Break in Scribus
  - _Insert > Spaces & breaks > Frame/Column break_

#### Color management

- 71. RGB vs CMYK
  - Some of the RGB colors cannot be printed
  - Activate the Color management and the out of Gamut warning
  - Colors in CMYK (in print!) are often less vibrant.
- 72. Using CMYK Color swatches in Scribus
  - When color management is active, Scribus warns for RGB colors that cannot be printed.
  - Editing colors.
  - Creating CMYK colors
- 73. RGB color spaces
  - Setting the color profile for images that have none sRGB being some kind of default / standard one).
- 74. Convert images to CMYK in Scribus
  - Correctly setting up the color management.
  - Target destination space is different in Europe (Fogra 39) and in the US (U.S. Web Coated).
- 75. Registration Black in Scribus
  - 100% of each C, M, Y, K: should never be used (except sometimes for registration marks)
- 76. Collect for Output in Scribus
  - For transering a project to a different computer, collect all resources of the project in a new folder.
- 77. Preflight Check in Scribus
  - Check the document for printing mistakes (missing images, low resolution, text overflow, objects not on a page)
  - Using _Manage Images_ to find missing images.

#### Pdf export

- 78. PDF versions
  - Pick the right PDF version in the preflight verifier.
  - Layers in PDF 1.6.
  - PDF X-variants need color management
  - ✎ Make sure that the print house does not introduce exceptions to the supported features in the accepted PDF versions (Typically: PDF 1.4 without transparencies)
- 79. Bleeds for single and facing pages in Scribus
  - For facing pages, the inner bleed should be zero.
- 80. Hiding Bleeds in a PDF
  - PDF sent to client for preview, should be optimized for screen viewing (no CMYK, no bleeds, lightweight).
- 81. Image Compression in Scribus
  - Target the monitor and reduce the image resolution in the PDF for preview or publishing on the web.
  - ✎ Not sure that the reccommendation to always outline the text is a good one.
- 82. Auto View PDF after exporting in Scribus
  - Adding the path to the PDF reader in the preferences.
- 83. PDF/X-4 vs PDF 1.6
  - Activating the color conversions also for PDF 1.6.

## Getting Started with Scribus by Top CLAX

<https://www.youtube.com/playlist?list=PLk8MAH_gd_XofdbK-1X_bczecCz5Mz6zK>

I've tested a _random_ introductory lesson ("Text frames") and it is shows multiple bad habits right at the start (creating text frames in columns without any guides, editing in the text editor).

I had also a very quick look at the first two lessons (install, overview) and it seems to have some mismatching details and then goes through big parts of the UI and basic features, without giving any clue on what is important and how to correctly use Scribus.

Scribus is a complex software and DTP is a complex task: This tutorials does not seem to do a good job at presenting Scribus in a way that helps the new user to get started and do a good job with it.

If I have some time, I will go through more of it, but from what I've seen, this tutorial series does not seem to be something I would recommend.

## Tutorials in French

- Ticeman de la Caverne:
  - [créer son premier document avec Scribus](https://www.youtube.com/watch?v=3ds9raf_agI)
  - [Importer une image dans Scribus et la modifier](https://www.youtube.com/watch?v=qn1_d-ZImrs)
    - Remarques:
      - Adapter le cadre à l'image avec le menu contextuel.
      - Aligner le cadre aux repères.
  - [Insérer et modifier du texte dans Scribus](https://www.youtube.com/watch?v=A8qh3Bs6mLI)
    - Problèmes:
      - Montre l'Éditeur de texte pour l'édition du texte (C'est mieux d'utiliser l'édition dans le cadre et la palette de propriétés)
  - [Appliquer une rotation aux éléments de Scribus](https://www.youtube.com/watch?v=XG4W83hU_44)
    - Problèmes:
      - Il faudrait aussi montrer l'outil de rotation.
  - [dégrouper un texte et le transformer en image dans Scribus](https://www.youtube.com/watch?v=eqWSnMCZTeM)
  - [Créer et appliquer des gabarits dans Scribus](https://www.youtube.com/watch?v=kLQUs6Jy22k)
    - Problèmes:
      - Il ne montre pas un usage correcte des gabarits (ça donne l'impression 
  - [Scribus: Modifier les bordures de cadres](https://www.youtube.com/watch?v=klC5CIj0hO4)
    - Problèmes:
      - Ne montre pas des bonnes habitudes (il met des cadres au hazard)
  - Qualités:
    - Montre de bons habitudes.
- IDIKOtv: Notions de mise en page:
  - [Techniques et pratique du graphisme et de l’infographie](https://www.youtube.com/watch?v=u8m6x1KJPcs)
  - [Texte et mise en page: assurer la lisibilité et l'esthétique d'un document](https://www.youtube.com/watch?v=73JBcnbOM8I)
  - [Objets ancrés: assurer la cohérence des images avec le texte](https://www.youtube.com/watch?v=pAVM0AtfFcU)
    - Problèmes:
      - Scribus n'a pas d'objets ancrés, mais les principes de placement sont tout de même valables.
  - [Les feuilles de styles: manipuler sa mise en forme sans risque](https://www.youtube.com/watch?v=ZhsqhUxbr5s)
  - [Anatomie du caractère: comprendre la typologie de la typographie](https://www.youtube.com/watch?v=u8m6x1KJPcs)
  - [Rééchantillonnage: manipuler la résolution d'une image](https://www.youtube.com/watch?v=IuKvxI1SJX4)
  - [Dimension de l'image: distinguer la taille, la définition et la résolution](https://www.youtube.com/watch?v=BvQ8TmWTT4M)
  - [Comprendre le vectoriel](https://www.youtube.com/watch?v=1TVG2XozXOs)
- [Des outils libres pour la création d'un journal](https://pascal-tic.org/blogue/des-outils-libres-pour-la-creation-d%E2%80%99un-journal/)
  - <https://www.calameo.com/read/0006619940867e7db22e8>

## Scripter

- [Python scripting with Scribus](https://opensource.com/sites/default/files/ebooks/pythonscriptingwithscribus.pdf)

## Hints for tutorial creators

- User interface
  - Please put the "Tools" toolbar on the left and disable the other toolbars.
