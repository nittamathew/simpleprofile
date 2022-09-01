<template>
    <div>
     <b-jumbotron>
      <div class="row">
            <div class="col-md-6">
                Name:
            </div>
            <div class="col-md-6">
                First Last
            </div>
        </div>
        <div class="row">
            <div class="col-md-6">
                Age:
            </div>
            <div class="col-md-6">
                
            </div>
        </div>
        <div class="row">
            <div class="col-md-6">
                Occupation:
            </div>
            <div class="col-md-6">
                Devops
            </div>
        </div>
    </b-jumbotron>
    <b-jumbotron>
        <div>
            <b-button v-b-toggle.collapse-1 class="m-1">Project 1</b-button>
            <b-collapse visible id="collapse-1">
                <b-card>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy 
                    text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has 
                    survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.</b-card>
            </b-collapse>
        </div>
        <div>
            <b-button v-b-toggle.collapse-2 class="m-2">Project 2</b-button>
            <b-collapse visible id="collapse-2">
                <b-card>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy 
                    text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has 
                    survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged
                </b-card>
            </b-collapse>
        </div>
        
    </b-jumbotron>
    </div>
</template>

<script>
    import { BJumbotron, BButton, BCollapse, BCard, VBToggle } from 'bootstrap-vue'

    export default {
        name: 'Dashboard',
        components: {
          BJumbotron,
          BButton,
          BCollapse,
          BCard
        },
        directives: {
            "b-toggle": VBToggle
        }
    }
</script>