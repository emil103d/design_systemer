<script>
  import Footer from "./Footer.svelte";
  import Badge from "./Badge.svelte";
  import Button from "./Button.svelte";
  import Card from "./Card.svelte";
  import ButtonwBadge from "./ButtonwBadge.svelte";
  import AvatarwIndicator from "./AvatarwIndicator.svelte";
</script>

<main>
  <section>
    <h2>A. Footer</h2>
    <Footer
      links1={["Branding", "Design", "Marketing", "Advertisement"]}
      links2={["About us", "Contact", "Jobs", "Press Kit"]}
      links3={["Terms of use", "Privacy policy", "Coockie policy"]}
    />
    <pre><code
        >&lt;script&gt; import Button from "./Button.svelte"; &lt;/script&gt;
        {'<Footer>links1={["Branding", "Design", "Marketing", "Advertisement"]}links2={["About us", "Contact", "Jobs", "Press Kit"]}links3={["Terms of use", "Privacy policy", "Coockie policy"]} </Footer>'}</code
      ></pre>
  </section>

  <section>
    <h2>B. Badge component</h2>
    <article>
      <h3>Defeault Badge</h3>
      <Badge>Badge</Badge>
      <pre><code>{" <Badge>Badge</Badge>"}</code></pre>
    </article>

    <article>
      <h3>Primary Badge</h3>
      <Badge type="primary">primary</Badge>
      <pre><code>{'<Badge type="primary">primary</Badge>'}</code></pre>
    </article>

    <article>
      <h3>Secondary Badge</h3>
      <Badge type="secondary">secondary</Badge>
      <pre><code>{'<Badge type="secondary">secondary</Badge>'}</code></pre>
    </article>

    <article>
      <h3>Accent Badge</h3>
      <Badge type="accent">Accent</Badge>
      <pre><code>{'<Badge type="accent">Accent</Badge>'}</code></pre>
    </article>

    <article>
      <h3>Ghost Badge</h3>
      <Badge type="ghost">ghost</Badge>
      <pre><code>{'<Badge type="ghost">ghost</Badge>'}</code></pre>
    </article>
  </section>

  <section>
    <h2>C. Button component</h2>

    <article>
      <h3>Defeault Button</h3>
      <Button>Button</Button>
      <pre><code>{"<Button>Button</Button>"}</code></pre>
    </article>

    <article>
      <h3>Primary Button</h3>
      <Button type="primary">Primary</Button>
      <pre><code>{'<Button type="primary">Primary</Button>'}</code></pre>
    </article>

    <article>
      <h3>Secondary Button</h3>
      <Button type="secondary">Secondary</Button>
      <pre><code>{'<Button type="secondary">Secondary</Button>'}</code></pre>
    </article>

    <article>
      <h3>Accent Button</h3>
      <Button type="accent">Accent</Button>
      <pre><code>{'<Button type="accent">Accent</Button>'}</code></pre>
    </article>

    <article>
      <h3>Ghost Button</h3>
      <Button type="ghost">Ghost</Button>
      <pre><code>{'<Button type="ghost">Ghost</Button>'}</code></pre>
    </article>

    <article>
      <h3>Link Button</h3>
      <Button type="link">Link</Button>
      <pre><code>{'<Button type="link">Link</Button>'}</code></pre>
    </article>
  </section>

  <section>
    <h2>D. Card component</h2>
    <Card title="Shoes !" />
    <pre><code>{'<Card title="Shoes !" />'}</code></pre>
  </section>

  <section>
    <h2>E. Button w Badge component</h2>
    <ButtonwBadge title="Inbox">
      <Badge type="primary">99+</Badge>
    </ButtonwBadge>
    <pre><code
        >{'<ButtonwBadge title="Inbox"><Badge type="primary">99+</Badge> </ButtonwBadge>'}</code
      ></pre>
  </section>

  <section>
    <h2>F. Avatar w indicator</h2>
    <article>
      <h3>Large avatar</h3>
      <AvatarwIndicator type="large" name="K" />
      <pre><code>{' <AvatarwIndicator type="large" name="K" />'}</code></pre>
    </article>

    <article>
      <h3>Medium avatar</h3>
      <AvatarwIndicator type="medium" mode="indicator" name="K" image="false" />
      <pre><code
          >{' <AvatarwIndicator type="medium" mode="indicator" name="K" image="false" />'}</code
        ></pre>
    </article>

    <article>
      <h3>Small avatar</h3>
      <AvatarwIndicator type="small" name="K" />
      <pre><code>{'<AvatarwIndicator type="small" name="K" />'}</code></pre>
    </article>

    <article>
      <AvatarwIndicator type="x-small" name="K" image="false" />
      <pre><code
          >{'<AvatarwIndicator type="x-small" name="K" image="false" />'}</code
        ></pre>
    </article>
  </section>
</main>

<style>
  /* .avatar {
    display: flex;
    align-items: center;
    gap: 20px;
  } */

  section {
    max-width: min(600px, 100% - 2rem);
    padding: 2rem;
    margin: 2rem;
    margin-right: auto;
    margin-left: auto;
    background: white;
    border-radius: 10px;
    box-shadow: 1.2px 3.1px 1.7px rgba(0, 0, 0, 0.014),
      2.8px 7.4px 4.2px rgba(0, 0, 0, 0.022),
      5.3px 14px 7.9px rgba(0, 0, 0, 0.03),
      9.4px 25px 14.1px rgba(0, 0, 0, 0.038),
      17.5px 46.8px 26.3px rgba(0, 0, 0, 0.049),
      42px 112px 63px rgba(0, 0, 0, 0.07);
  }

  article {
    padding: 2rem;
    margin: 2rem;
    border-radius: 10px;
    margin-right: auto;
    margin-left: auto;
    background: rgba(0, 0, 0, 0.022);
    box-shadow: 1.2px 3.1px 1.7px rgba(0, 0, 0, 0.014),
      2.8px 7.4px 4.2px rgba(0, 0, 0, 0.022),
      5.3px 14px 7.9px rgba(0, 0, 0, 0.03),
      9.4px 25px 14.1px rgba(0, 0, 0, 0.038),
      17.5px 46.8px 26.3px rgba(0, 0, 0, 0.049),
      42px 112px 63px rgba(0, 0, 0, 0.07);
  }

  pre {
    padding: 0.5rem 1rem;
    border-radius: 0.4rem;
    color: white;
    background: black;
    width: fit-content;
    white-space: pre-wrap;
  }
</style>
