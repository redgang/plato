<template>
  <div class="demo-misc">
    <c-image class="img1" src="images/logo.png"></c-image>
    <c-image class="img2" src="images/logo.png"
      width="500"
      height="500"></c-image>
    <c-pane>pane</c-pane>
    <c-flex-box>
      <c-flex-item>flex-item-1</c-flex-item>
      <c-flex-item>flex-item-2</c-flex-item>
      <c-flex-item>flex-item-3</c-flex-item>
    </c-flex-box>
    <c-cell>
      <c-icon class="c-cell-icon" :value="0xe619"></c-icon>
      <c-label class="c-cell-label">Label1</c-label>
      <c-value class="c-cell-value">
        <c-checkbox :value.sync="model2.value"></c-checkbox>
      </c-value>
    </c-cell>
    <c-cell>
      <c-icon :value="0xe606"></c-icon>
      <c-label>Label2</c-label>
      <c-value class="c-cell-value">
        <c-checkbox :value.sync="model1.value"></c-checkbox>
      </c-value>
    </c-cell>
  </div>
</template>

<script>
import CImage from 'components/c-image'
import CPane from 'components/c-pane'
import CCell from 'components/c-cell'
import CIcon from 'components/c-icon'
import CLabel from 'components/c-label'
import CValue from 'components/c-value'
import CCheckbox from 'components/c-checkbox'
import CFlexBox from 'components/c-flex-box'
import CFlexItem from 'components/c-flex-item'
export default {
  data () {
    return {
      model1: {
        label: 'Label',
        value: true
      },
      model2: {
        label: 'Label',
        value: 1
      }
    }
  },

  components: {
    CImage,
    CPane,
    CCell,
    CIcon,
    CLabel,
    CValue,
    CCheckbox,
    CFlexBox,
    CFlexItem
  }
}
</script>

<style src="styles/views/demo-misc"></style>
