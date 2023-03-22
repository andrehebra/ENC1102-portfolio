<script>
    import { Navbar, NavBrand, NavHamburger, NavUl, NavLi } from "flowbite-svelte";
</script>


<Navbar let:hidden let:toggle>
    <NavBrand href="/">
      <img
        src="https://flowbite.com/docs/images/logo.svg"
        class="mr-3 h-6 sm:h-9"
        alt="Flowbite Logo"
      />
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
        Composition II
      </span>
    </NavBrand>
    <NavHamburger on:click={toggle} />
    <NavUl {hidden}>
      <NavLi href="/" active={true}>Generating Inquiry</NavLi>
      <NavLi href="/about">Multiple ways of writing</NavLi>
      <NavLi href="/services">Information literacy</NavLi>
      <NavLi href="/pricing">Research genre production</NavLi>
      <NavLi href="/contact">Contributing knowledge</NavLi>
      <NavLi href="/contact">Revision</NavLi>
    </NavUl>
  </Navbar>