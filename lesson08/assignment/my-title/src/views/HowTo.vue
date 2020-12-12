<template>
<div class="row pb-5">
  <h1 class="col-12 pt-5 pb-5">How to Cook an Egg: 4 Methods</h1>
  <!--  <image v-for="image in images" v-bind:key="image.alt"></image>  -->
  <section class="col-sm-6">
    <div class="pb-5" v-for="technique in techniques" v-bind:key="technique.title">
      <image-custom :imageName="technique.img"></image-custom>
      <h3 class="mt-4 pb-1">{{technique.title}}</h3>
      <p>{{technique.contentA}}</p>
      <p>{{technique.contentB}}</p>
    </div>
  </section>
</div>
</template>

<script>
import image from '../components/Image.vue';
//import Header from '../components/Header.vue';
//import mixin from '../mixin';

export default {
  name: 'methods',
    components: {
      'image-custom': image
//    'method-header': Header
    },
  data () {
    return {
      techniques: [
        {title: "BOILED",
          img: 'hard-boiled.jpg',
          // Use a backslash after lines of text so Javascript knows the string is continued; otherwise, errors occur
          contentA: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod \
          tempor incididunt ut labore et dolore magna aliqua. In egestas erat imperdiet sed euismod.\
          Maecenas sed enim ut sem viverra aliquet eget sit amet. Libero volutpat sed cras ornare \
          arcu dui vivamus arcu. Egestas sed sed risus pretium quam vulputate dignissim. Leo urna \
          molestie at elementum eu facilisis sed. In aliquam sem fringilla ut morbi tincidunt augue. \
          Egestas diam in arcu cursus euismod quis viverra. Ut eu sem integer vitae. Arcu ac tortor \
          dignissim convallis aenean. At elementum eu facilisis sed odio morbi quis commodo. \
          Fringilla ut morbi tincidunt augue interdum velit euismod. Aliquam ultrices sagittis orci \
          a scelerisque purus semper eget duis.",
          contentB: "Sit amet luctus venenatis lectus magna fringilla urna porttitor. Habitasse \
          platea dictumst quisque sagittis purus sit amet volutpat. Gravida rutrum quisque non tellus \
          orci ac auctor. Ut sem viverra aliquet eget sit amet tellus cras adipiscing. Ultrices eros \
          in cursus turpis massa. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sed \
          blandit libero volutpat sed cras ornare arcu. Massa placerat duis ultricies lacus sed. \
          Ipsum suspendisse ultrices gravida dictum fusce ut placerat orci. Aliquet lectus proin nibh \
          nisl condimentum id venenatis a. Suspendisse potenti nullam ac tortor vitae purus faucibus \
          ornare. Sodales ut eu sem integer vitae justo eget. Maecenas volutpat blandit aliquam etiam \
          erat velit. Odio ut sem nulla pharetra diam. Duis at tellus at urna. Tempor orci dapibus \
          ultrices in iaculis nunc sed augue lacus. Hac habitasse platea dictumst quisque sagittis \
          purus sit. Arcu dictum varius duis at consectetur lorem donec. Adipiscing diam donec \
          adipiscing tristique risus nec feugiat in. Eu turpis egestas pretium aenean pharetra magna \
          ac placerat.",
        },
        {title: "SCRAMBLED",
          img: 'scrambled.jpg',
          contentA: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod \
          tempor incididunt ut labore et dolore magna aliqua. In egestas erat imperdiet sed euismod.\
          Maecenas sed enim ut sem viverra aliquet eget sit amet. Libero volutpat sed cras ornare \
          arcu dui vivamus arcu. Egestas sed sed risus pretium quam vulputate dignissim. Leo urna \
          molestie at elementum eu facilisis sed. In aliquam sem fringilla ut morbi tincidunt augue. \
          Egestas diam in arcu cursus euismod quis viverra. Ut eu sem integer vitae. Arcu ac tortor \
          dignissim convallis aenean. At elementum eu facilisis sed odio morbi quis commodo. \
          Fringilla ut morbi tincidunt augue interdum velit euismod. Aliquam ultrices sagittis orci \
          a scelerisque purus semper eget duis.",
          contentB: "Sit amet luctus venenatis lectus magna fringilla urna porttitor. Habitasse \
          platea dictumst quisque sagittis purus sit amet volutpat. Gravida rutrum quisque non tellus \
          orci ac auctor. Ut sem viverra aliquet eget sit amet tellus cras adipiscing. Ultrices eros \
          in cursus turpis massa. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sed \
          blandit libero volutpat sed cras ornare arcu. Massa placerat duis ultricies lacus sed. \
          Ipsum suspendisse ultrices gravida dictum fusce ut placerat orci. Aliquet lectus proin nibh \
          nisl condimentum id venenatis a. Suspendisse potenti nullam ac tortor vitae purus faucibus \
          ornare. Sodales ut eu sem integer vitae justo eget. Maecenas volutpat blandit aliquam etiam \
          erat velit. Odio ut sem nulla pharetra diam. Duis at tellus at urna. Tempor orci dapibus \
          ultrices in iaculis nunc sed augue lacus. Hac habitasse platea dictumst quisque sagittis \
          purus sit. Arcu dictum varius duis at consectetur lorem donec. Adipiscing diam donec \
          adipiscing tristique risus nec feugiat in. Eu turpis egestas pretium aenean pharetra magna \
          ac placerat.",
        },
        { title: "FRIED",
          img: 'overeasy.jpg',
          contentA: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod \
          tempor incididunt ut labore et dolore magna aliqua. In egestas erat imperdiet sed euismod.\
          Maecenas sed enim ut sem viverra aliquet eget sit amet. Libero volutpat sed cras ornare \
          arcu dui vivamus arcu. Egestas sed sed risus pretium quam vulputate dignissim. Leo urna \
          molestie at elementum eu facilisis sed. In aliquam sem fringilla ut morbi tincidunt augue. \
          Egestas diam in arcu cursus euismod quis viverra. Ut eu sem integer vitae. Arcu ac tortor \
          dignissim convallis aenean. At elementum eu facilisis sed odio morbi quis commodo. \
          Fringilla ut morbi tincidunt augue interdum velit euismod. Aliquam ultrices sagittis orci \
          a scelerisque purus semper eget duis.",
          contentB: "Sit amet luctus venenatis lectus magna fringilla urna porttitor. Habitasse \
          platea dictumst quisque sagittis purus sit amet volutpat. Gravida rutrum quisque non tellus \
          orci ac auctor. Ut sem viverra aliquet eget sit amet tellus cras adipiscing. Ultrices eros \
          in cursus turpis massa. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sed \
          blandit libero volutpat sed cras ornare arcu. Massa placerat duis ultricies lacus sed. \
          Ipsum suspendisse ultrices gravida dictum fusce ut placerat orci. Aliquet lectus proin nibh \
          nisl condimentum id venenatis a. Suspendisse potenti nullam ac tortor vitae purus faucibus \
          ornare. Sodales ut eu sem integer vitae justo eget. Maecenas volutpat blandit aliquam etiam \
          erat velit. Odio ut sem nulla pharetra diam. Duis at tellus at urna. Tempor orci dapibus \
          ultrices in iaculis nunc sed augue lacus. Hac habitasse platea dictumst quisque sagittis \
          purus sit. Arcu dictum varius duis at consectetur lorem donec. Adipiscing diam donec \
          adipiscing tristique risus nec feugiat in. Eu turpis egestas pretium aenean pharetra magna \
          ac placerat.",
        },
          {title: "POACHED",
          img: 'poached.jpg',
          contentA: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod \
          tempor incididunt ut labore et dolore magna aliqua. In egestas erat imperdiet sed euismod.\
          Maecenas sed enim ut sem viverra aliquet eget sit amet. Libero volutpat sed cras ornare \
          arcu dui vivamus arcu. Egestas sed sed risus pretium quam vulputate dignissim. Leo urna \
          molestie at elementum eu facilisis sed. In aliquam sem fringilla ut morbi tincidunt augue. \
          Egestas diam in arcu cursus euismod quis viverra. Ut eu sem integer vitae. Arcu ac tortor \
          dignissim convallis aenean. At elementum eu facilisis sed odio morbi quis commodo. \
          Fringilla ut morbi tincidunt augue interdum velit euismod. Aliquam ultrices sagittis orci \
          a scelerisque purus semper eget duis.",
          contentB: "Sit amet luctus venenatis lectus magna fringilla urna porttitor. Habitasse \
          platea dictumst quisque sagittis purus sit amet volutpat. Gravida rutrum quisque non tellus \
          orci ac auctor. Ut sem viverra aliquet eget sit amet tellus cras adipiscing. Ultrices eros \
          in cursus turpis massa. Mollis nunc sed id semper risus in hendrerit gravida rutrum. Sed \
          blandit libero volutpat sed cras ornare arcu. Massa placerat duis ultricies lacus sed. \
          Ipsum suspendisse ultrices gravida dictum fusce ut placerat orci. Aliquet lectus proin nibh \
          nisl condimentum id venenatis a. Suspendisse potenti nullam ac tortor vitae purus faucibus \
          ornare. Sodales ut eu sem integer vitae justo eget. Maecenas volutpat blandit aliquam etiam \
          erat velit. Odio ut sem nulla pharetra diam. Duis at tellus at urna. Tempor orci dapibus \
          ultrices in iaculis nunc sed augue lacus. Hac habitasse platea dictumst quisque sagittis \
          purus sit. Arcu dictum varius duis at consectetur lorem donec. Adipiscing diam donec \
          adipiscing tristique risus nec feugiat in. Eu turpis egestas pretium aenean pharetra magna \
          ac placerat.",
        }
      ],
      images: [
      {id: 1, src: require('../assets/hard-boiled.jpg'), alt:'Image of hard-boiled eggs'},
      {id: 2, src: require('../assets/scrambled.jpg'), alt:'Image of scrambled eggs'},
      {id: 3, src: require('../assets/overeasy.jpg'), alt:'Image of overeasy eggs'},
      {id: 4, src: require('../assets/poached.jpg'), alt:'Image of poached eggs'},
    ],
    //,
    //  images: [
    //    {imageOne: require('../assets/hard-boiled.jpg'), title: "Hard-boiled eggs",
    //     imageTwo: require('../assets/scrambled.jpg'),
    //     imageThree: require('../assets/overeasy.jpg'),
    //     imageFour: require('../assets/poached.jpg')
    //   }
    //  ]
    }
  }
//  ,
//  mixins: [mixin]
}
</script>

<!--

-->
