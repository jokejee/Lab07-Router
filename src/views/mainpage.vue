<script setup>
import newcard from '../components/Newcard.vue'
import { ref } from 'vue';
</script>

<template>
        <newcard></newcard>
        <div class="row g-5">
          <div class="col-md-8">
      
            <article class="blog-post">
              
            
            </article>
      
            <article class="blog-post">
              
            </article>
      
            <nav class="blog-pagination" aria-label="Pagination">
            </nav>
      
          </div>
      
      
      <!--Side bar-->
          
              
      
              <div>
                
                <ul class="list-unstyled">
                  <li>
                    <a class="d-flex flex-column flex-lg-row gap-3 align-items-start align-items-lg-center py-3 link-body-emphasis text-decoration-none border-top" href="#" v-for="(i,index) in Box_news" :key="index">
                    <svg class="bd-placeholder-img"  xmlns="http://www.w3.org/2000/svg" aria-hidden="true" preserveAspectRatio="xMidYMid slice" focusable="false">
                      <image :xlink:href="i.img" x="0" y="40" width="100px" />
                    </svg>
                      <div class="col-lg-8">
                        <h6 class="mb-0">{{i.name }}</h6>
                        <small class="text-body-secondary">{{i.data_time}}</small>
                      </div>
                    </a>
                  </li>
                </ul>
              </div>
            
          
      
      
      
      </div>
    
</template>
