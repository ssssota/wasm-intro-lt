<div>
  <slot />
</div>

<style>
  div {
    position: relative;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    background-color: var(--background-color);
    color: var(--font-color);
  }
  div :global(a) {
    color: var(--link-color);
  }
  @media print {
    div {
      page-break-after: always;
    }
  }
</style>
