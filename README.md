# Bootstrap OOSASS

There are a lot of SASS versions of Twitter Bootstrap – this one is different. It aims to harness to full power of SASS placeholders and OOSASS in order to allow you to do things like this :

```sass
@import bootstrap/progress-bars

.custom-class
  @extend %progress
  article
    @extend %progress-bar
    @extend %progress-striped
    width: 20%
    &.other-class
    &:nth-child(3n)
      @extend %progress-active
```

No unsemantic OOCSS clutter of classes ; no full Bootstrap CSS to include when you only require one modules or two.
You handpick what you want and distribute it amongst **your** classes and **your** tags.
