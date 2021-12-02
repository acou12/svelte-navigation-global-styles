<script>
  function dynamicallyGeneratedContent() {
    return "<p>Dynamically generated content</p>";
  }
</script>

<p>{@html dynamicallyGeneratedContent()}</p>
<p>Now press the back button.</p>

<style>
  :global(p) {
    color: pink;
  }
  /*
  Doesn't work; the style is not applied to 
  the dynamically generated content.
  
  p {
    color: pink;    
  } */
</style>