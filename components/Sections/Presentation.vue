<template>
  <div class="my-auto">
    <h1 class="mb-0">
      {{ $t('personalInfo.name') }}
      <span class="text-primary">{{ $t('personalInfo.lastName') }}</span>
    </h1>

    <h3 class="mb-4">
      <vue-typer
        :text="$t('personalInfo.subHeadingText')"
        :repeat="Infinity"
        :shuffle="true"
        initial-action="typing"
        :pre-type-delay="100"
        :type-delay="82"
        :pre-erase-delay="2000"
        :erase-delay="30"
        erase-style="backspace"
        :erase-on-complete="false"
        caret-animation="blink"
      ></vue-typer>
    </h3>

    <div class="subheading mb-5">
      {{ $t('personalInfo.city') }} ·
      <a :href="'mailto:' + $t('personalInfo.email')">{{ $t('personalInfo.email') }}</a>
    </div>
    <p class="mb-5">
      {{ $t('personalInfo.myDescription') }}
    </p>
    <ul class="list-inline list-social-icons mb-0">
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.linkedin')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-linkedin-in fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.github')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-github-alt fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.stackshare')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-stack-exchange fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.instagram')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-instagram fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.flickr')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-flickr fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>
