# CKEditor Quick Start Guide

The aim of this article is to get you up and running with CKEditor in two minutes.

## Download

Visit the official [CKEditor Download](http://ckeditor.com/download) site. For a production site we recommend you choose the default **Standard Package** and click the **Download CKEditor** button to get the `.zip` installation file. If you want to try out more editor features, you can download the **Full Package** instead.

<a href="http://ckeditor.com/download"><img src="guides/dev_installation/ckeditor_quick_start_download.png" alt="CKEditor Download site" width="696" height="321"></a>

## Unpacking

Unpack (extract) the downloaded `.zip` archive to the `ckeditor` directory in the root of your website.

## Trying Out

CKEditor comes with a collection of samples that you can try out to verify if the installation was successful as well as see some CKEditor usage scenarios, both basic and more advanced.

Open the following page in the browser:
`http://<your site>/ckeditor/samples/index.html`

Browse the samples to see how CKEditor can be used and customized.

## Adding CKEditor to Your Page

If the samples work correctly, you are ready to build your own site with CKEditor included.

To start, create a simple HTML page with a `<textarea>` element in it. You will then need to do two things:

1. Add a call to the CKEditor script in the `<script>` element of your page.
2. Use the [`CKEDITOR.replace()`](#!/api/CKEDITOR-method-replace) method to  replace the existing `<textarea>` element with CKEditor.

See the following example:

	<!DOCTYPE html>
	<html>
		<head>
			<title>A Simple Page with CKEditor</title>
			<!-- Make sure the path to CKEditor is correct. -->
			<script src="../ckeditor.js"></script>
		</head>
		<body>
			<form>
				<textarea id="editor1" name="editor1" rows="10" cols="80">
					This is my textarea to be replaced with CKEditor.
				</textarea>
				<script>
					// Replace the <textarea id="editor1"> with a CKEditor
					// instance, using default configuration.
					CKEDITOR.replace( 'editor1' );
				</script>
			</form>
		</body>
	</html>

When you are done, open your sample page in the browser.

**Congratulations! You have just installed and used CKEditor on your own page in virtually no time!**

<img src="guides/dev_installation/ckeditor_on_page.png" alt="CKEditor added to your sample page" width="483" height="252">

## Next Steps

Go ahead and play a bit more with the samples; try to add the same functionality to your own pages (you can always see the sample source for some hints). And when you are ready to dive a bit deeper into CKEditor, you can try the following:

1. Check the [Configuration](#!/guide/dev_configuration) section to see how to adjust the editor to your needs.
2. [Modify your toolbar](#!/guide/dev_toolbar) to only include the features that you need. You can find the complete list of all toolbar buttons available in your build in the "Toolbar Configurations" sample.
3. Browse the [Add-ons Repository](http://ckeditor.com/addons/plugins/all) for some additional plugins or skins.
4. Use [CKBuilder](http://ckeditor.com/builder) to create your custom CKEditor build.
5. Browse the [Developer's Guide](#!/guide) for some further ideas on what to do with CKEditor and [join the community](http://ckeditor.com/forums) to discuss all things CKEditor with fellow developers!