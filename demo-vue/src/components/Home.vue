<template>
  <Page class="page">
    <ActionBar class="action-bar" title="Home"/>
    <GridLayout rows="40, auto, *, 50">
      <Label row="0" text="Text on the page in row 1 of grid" color="green" textWrap="true"></Label>
      <GridLayout row="2">
          <Carousel #carousel ios:indicatorOffset="0,-10" ios:finite="true" ios:bounce="false" showIndicator="true" height="100%" indicatorAnimation="SWAP"
              indicatorColor="#66ccff" indicatorColorUnselected="#cceeff" width="80%">
              <CarouselItem backgroundColor="red" height="100%">
                  <Label class="h2 text-center" color="white" textWrap="true" text="1"></Label>
              </CarouselItem>
              <CarouselItem backgroundColor="purple">
                  <Label class="h2 text-center" color="white" textWrap="true" text="2"></Label>
              </CarouselItem>
          </Carousel>
      </GridLayout>
      <Label row="3" text="After 5 seconds the indicator animation will change to WORM on ANDROID" textWrap="true"></Label>
    </GridLayout>

  </Page>
</template>
