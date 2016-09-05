# HydrOS: A massively fault tolerant operating system

HydrOS is a multikernel research operating system written to withstand complete software failure, as well as partial hardware failure, in Erlang. HydrOS uses the multikernel model to seperate a multicore computer into a set of individual computing nodes, each capable of withstanding the failure of the others.

Each node runs a lightly modified BEAM virtual machine as it's kernel, with the operating system and hosted programs written in Erlang.

## Try it out

Download the latest version (version 0.01) here.

Once the image is unpacked, simple open it in a supported virtual machine (examples listed below), or write the image to a USB stick and run it on a real computer.

Please note that this is research software, not yet ready for real deployment. Use at your own risk!

## Host Requirements

HydrOS runs on all physical machines tested. It has also been tested in the following virtual environments:

* Bochs
* Qemu
* KVM

Unfortunately, VirtualBox is not supported at this time.

## Building

1. Please download the latest source archive here.
2. Build a cross-compiler toolchain that targets `x86_64-unknown-elf` with `crosstool-ng`
3. Run `make` in the HydrOS root directory.
4. Either write the `build/hydros.img` file to a USB drive for testing, or run the OS in a virtual machine.

## Keep up to date

Join our mailing list to hear about new releases of HydrOS. We will not to give your email address to any third parties, aside our list manager, MailChimp.

<!-- Begin MailChimp Signup Form -->
<link href="//cdn-images.mailchimp.com/embedcode/slim-10_7.css" rel="stylesheet" type="text/css">
<style type="text/css">
	#mc_embed_signup{background:#fff; clear:left; font:14px Helvetica,Arial,sans-serif; }
	/* Add your own MailChimp form style overrides in your site stylesheet or in this style block.
	   We recommend moving this block and the preceding CSS link to the HEAD of your HTML file. */
</style>
<div id="mc_embed_signup">
<form action="//hydros-project.us14.list-manage.com/subscribe/post?u=d6d4d8a6c17506b92aedd38de&amp;id=501a91e678" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
<div id="mc_embed_signup_scroll">
	
<input type="email" value="" name="EMAIL" class="email" id="mce-EMAIL" placeholder="email address" required>
<div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_d6d4d8a6c17506b92aedd38de_501a91e678" tabindex="-1" value=""></div>
<div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
</div>
</form>
</div>

<!--End mc_embed_signup-->
