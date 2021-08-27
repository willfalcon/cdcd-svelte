<script>
	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	:global(:root) {
		--orange: #F5591F;
		--lightOrange: #F5911F;
		--offWhite: white;
		--dark: #4E4D39;
		--grey: #979797;
		--light: #F7F7F3;
		--black: #3C3837;
		--darkBlue: #31363B;
		--red: #C60606;
		--green: #008E02;
		--fontSans: granville, serif;
		--font: granville, serif;
		--fontHeading: degular, sans-serif;
		--fontBook: 300;
		--fontRegular: 400;
		--fontBold: 700;
		--fontBlack: 900;
	}
	:global(html) {
    box-sizing: border-box;
    font-size: 10px;
    -ms-overflow-style: -ms-autohiding-scrollbar;
  }
  :global(*, *:before, *:after) {
    box-sizing: inherit;
  }
  :global(:focus) {
    outline-color: var(--lightOrange);
  }
  :global(body) {
    padding: 0;
    margin: 0;
    font-family:var(--font);
    font-weight: 400;
    font-style: normal;
    font-size: 1.6rem;
    line-height: 2;
    background-color: var(--light);
    color: var(--dark);
    min-height: 100vh;
    /* @media (prefers-color-scheme: dark) {
      background-color: ${({ theme }) => theme.dark};
      color: ${({ theme }) => theme.offWhite};
    }  */
  }
  :global(img) {
    display: block;
		max-width: 100%;
		height: auto;
  }
  :global(h1) {
    font-family: var(--fontHeading);
    font-weight: var(--fontBlack);
  }
  :global(h2) {
    font-family: var(--fontHeading);
    line-height: 1.25;
    margin: 0;
    font-size: 2.8rem;
  }
  :global(h3, label, input, textarea) {
    font-family: var(--fontHeading);
    font-weight: 700;
    font-style: normal;
    letter-spacing: 2px;
    line-height: 2.15;
    margin: 0 0 .5rem;
    font-size: 1.6rem;
  }
  :global(h4) {
    /* font-family: , sans-serif; */
    font-family: var(--fontHeading);
    font-weight: 700;
    font-style: normal;
    letter-spacing: 2px;
  }
  :global(label) {
    color: var(--dark);
  }
  :global(p) {
    margin: 0 0 1rem;
    font-size: 1.6rem;
  }
  :global(.text-center) {
    text-align: center;
  }
  :global(.loading-indicator-appear,
  .loading-indicator-enter) {
    opacity: 0;
  }
  :global(.loading-indicator-appear-active,
  .loading-indicator-enter-active) {
    opacity: 1;
    transition: opacity 400ms;
  }
  :global(.flag) {
    color: var(--red);
  }
	
</style>