---
layout: default 
permalink: /reading/
title: "Reading"
---

<p id="feed"></p>

<script>
<!--
$(document).ready(function(){
var id = '1-QNbUp7N_FMLEk24dgCQVNVvhIvjmer_67r34Vtfbi8';
var url = "https://spreadsheets.google.com/feeds/list/" + id + "/od6/public/values?alt=json";
function hostname(url) {
  var matches = url.match(/^https?\:\/\/(www\.)?([^\/?#]+)(?:[\/?#]|$)/i);
    return matches[2];
    }
    $.getJSON(url, function(data) {
      var feed = '';
        $($(data.feed.entry).get().reverse()).each(function(){
            var quote = '', excerpt = this.gsx$excerpt.$t;
                if (excerpt && !/\u2026$/.test(excerpt))
                        quote = '<br>"' + excerpt + '"';
                            feed += '<p><b><a href="' + this.gsx$url.$t + '">' + this.gsx$title.$t + '</a></b>'
                                        + ' <i>@' + hostname(this.gsx$url.$t) + '</i>' + quote + '</p>';
                                          });
                                            $('#feed').append(feed);
                                            });
                                            }); /* ready */
                                            //-->
                                            </script>