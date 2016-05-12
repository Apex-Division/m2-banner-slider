# m2-banner-slider
Copied from https://github.com/emizentech/magento2-banner-slider

<h3>Notes:</h3>
<ul>
<li>Modified composer.json to make it compatible with Magento 2.0.5</li>
<li>Modified widget.xml to prevent admin console errors</li>
<li>Even the namespace is kept same</li>
</ul>

<h2>Composer Installation Instructions</h2>
Add GIT Repository to composer
<pre>
composer config repositories.apexdivision-m2-banner-slider vcs https://github.com/Apex-Division/m2-banner-slider/
</pre>

Since this package is in a development stage, you will need to change the minimum-stability as well to the composer.json file: -
<pre>
"minimum-stability": "dev",
</pre>

After that, need to install this module as follows:
<pre>
  composer require magento/magento-composer-installer
  composer require apexdivision/apexdivision-m2-banner-slider
</pre>


<br/>
<h2> Mannual Installation Instructions</h2>
go to Magento2Project root dir 
create following Directory Structure :<br/>
<strong>/Magento2Project/app/code/Emizentech/Banner</strong>
you can also create by following command:
<pre>
cd /Magento2Project
mkdir app/code/Emizentech
mkdir app/code/Emizentech/Banner
</pre>



<h3> Enable Emizentech/Banner Module</h3>
to Enable this module you need to follow these steps:

<ul>
<li>
<strong>Enable the Module</strong>
<pre>bin/magento module:enable Emizentech_Banner</pre></li>
<li>
<strong>Run Upgrade Setup</strong>
<pre>bin/magento setup:upgrade</pre></li>
<li>
<strong>Re-Compile (in-case you have compilation enabled)</strong>
	<pre>bin/magento setup:di:compile</pre>
</li>
</ul>