TestFairy provides methods for identifying, or tagging, users who use your app. Often you would be interested in searching based on a specific user-id, or attributes.

Sample use cases:

- Search for recordings by john@example.com
- Search for recordings

<div align="right" style="margin-bottom: 8px;">
	Framework: <select id="x">
		<option value="android" selected>Android</option>
		<option value="objective-c">iOS Objective-C</option>
		<option value="swift">iOS Swift</option>
		<option value="cordova">Cordova</option>
		<option value="unity">Unity</option>
		<option value="react-native">React-Native</option>
		<option value="nativescript">Nativescript</option>
	</select>
</div>

<div data-framework="android" style="display: none;">
<pre>
TestFairy.setUserId("john@example.com");
</pre>
</div>

<div data-framework="objective-c" style="display: none;">
<pre>
[TestFairy setUserId:@"john@example.com"];
</pre>
</div>

<div data-framework="cordova" style="display: none;">
<pre>
TestFairy.setUserId("john@example.com");
</pre>
</div>

<div data-framework="nativescript" style="display: none;">
<pre>
TestFairySDK.setUserId("john@example.com");
</pre>
</div>

<div data-framework="unity" style="display: none;">
<pre>
TestFairy.setUserId("john@example.com");
</pre>
</div>

<div data-framework="react-native" style="display: none;">
<pre>
componentWillMount: function() {
    TestFairy.setUserId("john@example.com");
}
</pre>
</div>

<style>.content-page pre { margin-right: 0; }</style>
<style>.content-page pre { border-radius: 4px; }</style>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script>$(document).ready(function(){  function onFrameworkChanged() { var framework = $("select#x").val(); $("div[data-framework]").hide(); $("div[data-framework=" + framework + "]").show(); }       $("select#x").change(onFrameworkChanged);   onFrameworkChanged(); });</script>
