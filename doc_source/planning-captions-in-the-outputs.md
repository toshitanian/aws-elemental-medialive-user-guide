# Step 2: Plan Captions for the Outputs<a name="planning-captions-in-the-outputs"></a>

If you followed the instructions in [[ERROR] BAD/MISSING LINK TEXT](identify-captions-in-the-input.md), you should have a list of the caption formats and languages that will be available for inclusion in the outputs\. 

You must now plan the caption information for the outputs:

1. Identify the types of output media that you plan to create in the channel\. For example, Microsoft Smooth and HLS\.

1. Identify the combinations of video and audio that you plan to create for each output media\. 

1. For each output media, identify which input captions will be converted to which output formats\. For example, you will convert teletext captions to TTML for the Microsoft Smooth output media, and those same teletext captions to Web\-VTT for the HLS output media\. 

   The output formats that are possible depend on the input formats and the type of output media\. See [[ERROR] BAD/MISSING LINK TEXT](supported-captions.md) to determine which output captions are possible given the input format\. 

1. Identify the languages for each output format:

   + In general, count each language separately\. 

   + Exception: For embedded\-to\-embedded, count all languages as one\. 

   + Exception: For teletext\-to\-teletext, count all languages as one\.

*The Result*

You end up with a list of outputs, and the captions formats and languages for each output\. For example:

+ Microsoft Smooth output with TTML captions in Czech

+ Microsoft Smooth output with TTML captions in Polish

+ HLS output with Web\-VTT captions in Czech

+ HLS output with Web\-VTT captions in Polish

## Outputting Multiple Formats<a name="output-multiple-formats"></a>

You can include captions from two or more different formats in an output\. For example, you can include both embedded captions and WebVTT captions in an HLS output, to give the downstream system more choices about which captions to use\. The only rules for multiple formats are the following:

+ The output container must support all the formats\. See [[ERROR] BAD/MISSING LINK TEXT](supported-captions.md)\.

+ The font styles in all the captions that are associated with an output must match\. This means that the end result must be identical, not that you must use the same option to get that result\. For example, all captions that are associated with the output must be white for the first language and blue for the second language\.

Managing this style matching can be a little tricky\. For information about the font style options, see [Support for Font Styles in Output Captions](support-for-font-styles-in-output-captions.md)\.