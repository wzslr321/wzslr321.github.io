<script>
  import SectionHeader from '../Main/SectionHeader.svelte'
</script>

<section>

    <SectionHeader textContent="My Experience"/>

    <section>
        <a href="https://github.com/wzslr321" target="_blank">
            <picture>
                <img src="images/github-icon.webp" alt="Github Icon" width="100%" height="100%"/>
            </picture>
        </a>
        <article>
            I don't have projects that run live in the web. So far I have been focusing
            on personal projects with an emphasis on self improvement.
            Check out my
            <a href="https://github.com/wzslr321">
                <span class="highlighted-text">
                    Github Profile
                </span>
            </a>
            with all the public code I wrote so far!
        </article>
    </section>
</section>

<style lang="scss">
  @import 'public/style/variables.scss';

  section {
    section {

      max-width: $container-width;
      margin: 0 auto;
      padding: $horizontal-padding 0;
      display: flex;
      font-size: 1.3em;
      align-items: center;

      article {
        padding: 0 6em;
        text-shadow: 2px 2px 2px black;

        a {
          text-decoration: none;
        }

        a:hover {
          transition: 0.5s;
          font-size: 1.025em;
        }
      }
    }
  }

  @media(max-width: 992px) {
    section {
      section {
        max-width: 100%;
        padding:0 1em;
        a {
          display:none;
        }

        article{
          padding:0 1em;
          text-align:center;
          a {
            display: inline;
          }
        }
      }
    }
  }

</style>
