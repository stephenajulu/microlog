<template>
	<div class="author">
	
	<g-image
      alt="Author image"
      class="author__image"
      src="~/assets/images/author.jpg"
      width="180"
      height="180"
      blur="5"
    />

		<h1 v-if="showTitle" class="author__site-title">
			{{ $static.metadata.siteName }}
		</h1>

		<p class="author__intro">
			Hi There!
		<br>
			How are you? I'm Stephen Ajulu. I am a Student, Front End Web Developer, Graphic Designer, Junior Cybersecurity Consultant and Content Creator Based in Nairobi, Kenya.
		</p>

		<p class="author__links">
		
		<a href="//twitter.com/stephenajulu"><g-image alt="twitter" class src="~/assets/images/twitter.png"/></a>
      		<a href="//dev.to/stephenajulu"><g-image alt="dev" class src="~/assets/images/dev.jpg" width="30"/></a>
                <a href="//instagram.com/stephenajulu"><g-image alt="instagram" class src="~/assets/images/instagram.png"/></a>
       		<a href="/rss.xml"><g-image alt="rss" class src="~/assets/images/rss.png" width="30"/></a>
      		<a href="//github.com/stephenajulu"><g-image alt="github" class src="~/assets/images/github.png"/></a>
      		<a href="//linkedin.com/in/stephenajulu"><g-image alt="linkedin" class src="~/assets/images/linkedin.png" width="32"/></a>
      		<!-- <a href="//noti.st/stephenajulu"><g-image alt="notist" class src="~/assets/images/notist.jpg" width="32"/></a> -->
		
		</p>

	</div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
export default {
	props: ['showTitle']
}
</script>

<style lang="scss">
.author {
	margin: 0 auto;
	max-width: 500px;
	text-align: center;
	padding-bottom: calc(var(--space) / 2);

	&__image {
		border-radius: 100%;
		width: 90px;
		height: 90px;
		margin-bottom: 1em;
	}

	&__intro {
		opacity: .8;
	}

	&__site-title {
		margin: 0 auto;
		font-size: 1.5em;
		max-width: 400px;
	}

	&__links {
		margin-top: -.5em;
		a {
			margin: 0 .5em;
		}
	}
}
</style>
