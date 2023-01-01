<div>
    <TabBar tabs={['Home', 'Merchandise', 'About Us']} let:tab bind:active>
        <Tab {tab} href="#{tab.replace(/ /g, '_').toLowerCase()}">
            <Label>{tab}</Label>
        </Tab>
    </TabBar>
</div>
  
<script lang="ts">
    import Tab, { Label } from '@smui/tab';
    import TabBar from '@smui/tab-bar';

    let active = 'Home';
</script>
