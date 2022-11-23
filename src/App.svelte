<script lang="ts">
  import { FormGroup, Label, Input, Icon, Button } from "sveltestrap";
  let text: string = "t";
</script>

<main>
  <FormGroup>
    <Label for="exampleText">Text Area</Label>
    <Input type="textarea" name="text" id="exampleText" bind:value={text} />
  </FormGroup>
  <div class="d-grid gap-3">
    <div class="output-textbox border round">
      <sub>{text}</sub>
      <!--
      <Button>
        <Icon name="clipboard" />
      </Button>
      -->
    </div>
    <div class="output-textbox border round">
      <sup>{text}</sup>
      <!--
      <Button>
        <Icon name="clipboard" />
      </Button>
      -->
    </div>
  </div>
</main>
