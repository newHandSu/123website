<template>
    <div class="home-box">
        <div class="banner-box u-banner">

        </div>

        <div class="con-box">
            <div class="login">
                <div class="title u-center">免费申请体验课</div>
                <div class="form">
                    <div class="i-tit p-t25">小朋友的姓名：</div>
                    <input type="text" class="ipt" v-model="name" />
                    <div class="i-tit">您的联系方式：</div>
                    <input type="text" class="ipt" v-model.number="phone" maxlength="11" />
                    <div class="i-tit">小朋友的年龄（岁）：</div>
                    <input type="text" class="ipt" v-model="age" />
                    <div class="u-btn" @click="submit">申请提交</div>
                    <div class="swipe u-center">{{text}}</div>
                </div>
            </div>

            <div class="g1 mt10">
                <div class="title-bg title-text">123足球理念——三条“大鱼”</div>
                <div class="imgs clearfix">
                    <div class="f-left">
                        <img src="./images/h1.png" alt="">
                        <div class="bt">
                            <span class="da">教育</span>大于足球
                        </div>
                    </div>
                    <div class="f-left">
                        <img src="./images/h2.png" alt="">
                        <div class="bt">
                            <span class="da">成长</span>大于成绩
                        </div>
                    </div>
                    <div class="f-left">
                        <img src="./images/h3.png" alt="">
                        <div class="bt">
                            <span class="da">自动</span>大于外力
                        </div>
                    </div>
                </div>
            </div>
            <div class="g2 mt10">
                <div class="title-bg title-text">123足球的核心</div>
                <div class="qa-box">
                    <div class="q-tit red">
                        <span class="da">意识：</span>在所有年龄段的孩子，指导珍惜以下4 种心理成长
                    </div>
                    <div class="q-con q-red">
                        <p>1、礼貌：礼节，包括寒暄，感谢，和用语（能够在适当的时候说正确的话）；</p>
                        <p>2、主体性：发生状况后能够自己开动脑筋去解决问题；</p>
                        <p>3、协调性：将就团体的—比如集体行动，遵守规则，有道歉的心（为团队或者其他队友着想）等等；</p>
                        <p>4、挑战精神：不放弃，拼尽全力。</p>
                    </div>

                    <div class="q-tit gree">
                        <span class="da">球：</span>通过观察，并结合年龄和发展心理学的规律，制定课程重心
                    </div>
                    <div class="q-con q-gree">
                        <p>1、3-6岁：自己和球；</p>
                        <p>2、7-8岁：自己和球还有对手。让他们理解这些内容；</p>
                        <p>3、9-12岁：自己和球和对手和队友，最后是球场空间的理解和掌握。</p>
                    </div>

                    <div class="q-tit blue">
                        <span class="da">身体：</span>要观察和考虑到各年龄儿童的身体、骨骼发育规律和特点，制定合理的课程训练侧重点
                    </div>
                    <div class="q-con q-blue">
                        <p>1、3-6岁：多样的基本动作（敏捷性，平衡性，细致性）；</p>
                        <p>2、7-8岁：把多样的基本动作做不同的组合；</p>
                        <p>3、9-10岁：足球的专门东西（基本）；</p>
                        <p>4、11-12岁：足球的专门动作（应用型）。</p>
                    </div>
                </div>
            </div>
            <div class="g3 mt10">
                <div class="title-bg title-text">123足球——入会流程</div>
                <div class="st1 clearfix c-01">
                    <div class="con-01 left">
                        <div class="da">STEP 01</div>
                        <div class="ms">申请免费体验课</div>
                    </div>
                    <div class="left img"></div>
                    <div class="tips left">
                    首先参加免费体验课。由于需要提前申请，请通过线上登记信息、线上提交申请表、电话联系人工登记信息等形式预约体验课。我们会在最快时间与您取得电话联系；
                    </div>
                </div>

                <div class="st1 clearfix c-02">
                    <div class="con-01 left">
                        <div class="da">STEP 02</div>
                        <div class="ms">参加免费体验课</div>
                    </div>
                    <div class="left img"></div>
                    <div class="tips left">
                    在参加免费体验课时，将为您提供入会相关协议；
                    </div>
                </div>

                <div class="st1 clearfix c-03">
                    <div class="con-01 left">
                        <div class="da">STEP 03</div>
                        <div class="ms">提交入会协议 <br />缴纳相关学费</div>
                    </div>
                    <div class="left img"></div>
                    <div class="tips left">
                    填写入会申请协议，并交纳相关费用；
                    </div>
                </div>

                <div class="st1 clearfix c-04">
                    <div class="con-01 left">
                        <div class="da">STEP 04</div>
                        <div class="ms">入会完成</div>
                    </div>
                    <div class="left img"></div>
                    <div class="tips left">
                    提交入会申请协议，完成登记信息，公司会员服装、足球等邮寄工作、入会完成！
                    </div>
                </div>

                <div class="sq-box">
                    <div class="sq-btn">0元申请体验</div>
                </div>
            </div>
            <div class="g4 mt10">
                <div class="title-bg title-text">123足球——合作伙伴</div>
                <div class="ms">与123足球一起，助力亿万孩子的足球梦</div>
                <div class="imgs-box">
                    <div v-for="img in imgs" :key="img" class="hz-logo">
                        <img src=""  />
                        <div class="hz-tit">xxx</div>
                    </div>
                </div>

                <div class="sq-box">
                    <div class="u-btn">更多关于我们</div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Vue from 'vue';
import { Message } from 'element-ui';
import Util from '../../common/tools/ajax';


Vue.component(Message.name, Message);

export default {
  name: 'home',
  data() {
    return {
      imgs: [1, 2, 3, 4, 5, 6, 7, 8, 9],
      name: '',
      phone: '',
      age: '',
      text: '135****306家长申请体验课成功！180****415',
    };
  },
  methods: {
    submit() {
      const { name, age, phone } = this;

      if (!name || !age || !phone) {
        return Message({
          message: '请填写完整的用户信息',
          type: 'error',
          duration: 4000,
          center: true,
        });
      }

      Util.api({
        url: 'front/addExperienceUser',
        method: 'POST',
        data: {
          childName: name,
          age,
          mobile: phone,
          childSex: '男',
          nearCenterAddress: '无',
        },
      }).then((res) => {
        if (res.code === 0) {
          this.name = '';
          this.age = '';
          this.phone = '';
          Message({
            message: '预约成功!',
            type: 'success',
            duration: 4000,
            center: true,
          });
        }
      });
    },
  },
};
</script>
<style scoped lang="less">
@import "../../../static/css/index.less";
@import "./index.less";
</style>
