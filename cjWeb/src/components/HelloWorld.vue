<template>
  <!-- <h1>{{ msg }}</h1>
  <button @click="count++">count is: {{ count }}</button>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p> -->
  <div></div>
</template>

<script>
import { Workbook, Topic, Marker, Zipper } from 'xmind';
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      count: 0
    }
  },
  mounted(){
    console.log(Workbook, Topic, Marker, Zipper)

    // const [ workbook, marker ] = [new Workbook(), new Marker()];

    // const topic = new Topic({sheet: workbook.createSheet('sheet title', 'Central Topic')});
    // const zipper = new Zipper({path: '/tmp', workbook, filename: 'MyFirstMap'});

    // // topic.on() default: `central topic`
    // topic.add({title: 'main topic 1'});

    // topic
    //   .on(topic.cid(/*In default, the componentId is last element*/))
      
    //   // add subtopics under `main topic 1`
    //   .add({title: 'subtopic 1'})
    //   .add({title: 'subtopic 2'})
      
    //   // attach text note to `main topic 1`
    //   .note('This is a note attached on main topic 1')
      
    //   // attach a marker flag to `subtopic 1`
    //   .on(topic.cid('subtopic 1'))
    //   .marker(marker.week('fri'))
      
    //   // add a component of the summary that contains two sub topics
    //   .summary({title: 'subtopic summary', edge: topic.cid('subtopic 2')})
      
    // zipper.save().then(status => status && console.log('Saved /tmp/MyFirstMap.xmind'));

  }
}
</script>
