<script setup></script>
<template>
  <div class="wrapper">
    <div class="header-box">
      <img
        src="https://image.winudf.com/v2/image1/Y29tLnNhYnVkaS5ncHQzLmNoYXQuYWlfaWNvbl8xNjcxNTIyMzAwXzA4NQ/icon.png?fakeurl=1&amp;h=240&amp;type=webp"
        alt="Logo"
        class="logo"
      />
    </div>
    <div class="content-box">
      <div class="section section1">
        <div class="user-box">
          <div class="user-head">
            <img src="https://via.placeholder.com/80x80" alt="user-image" />
            <span class="user-name">John</span>
          </div>
          <ul class="user-body">
            <li>
              <span>性別</span>
              <span>男</span>
            </li>
            <li>
              <span>年齡</span>
              <span>25</span>
            </li>
            <li>
              <span>身高</span>
              <span>175 cm</span>
            </li>
            <li>
              <span>體重</span>
              <span>70 kg</span>
            </li>
            <li>
              <span>BMI</span>
              <span>22.9</span>
            </li>
            <li>
              <span>基礎代謝率</span>
              <span>1500 kcal/day</span>
            </li>
          </ul>
        </div>
        <div class="info-txt">
          <div class="title">基礎代謝率(BMR)：</div>
          <div class="content">
            基礎代謝率(Basal Metabolic
            Rate)即為身體需要維持運作、休息、維持生命所消耗的最低能量，BMR的計算方式男女有些微差異。<br />BMR男：10*KG+6.25*CM-5*年紀+5
            <br />BMR女：10*KG+6.25*CM-5*年紀-161
          </div>
          <div class="title">身體質量指數(BMI)：</div>
          <div class="content">
            體重過輕：BMI &lt; 18.5<br />正常範圍：18.5 ≤ BMI &lt; 24<br />體重過重：24
            ≤ BMI &lt; 27<br />肥胖：BMI ≥ 27<br />BMI = 體重(公斤) /
            身高2(公尺2)
          </div>
        </div>
      </div>
      <div class="section section2">
        <div class="bmr-info">
          <h2>每日總熱量消耗 (TDEE)</h2>
          <p>
            TDEE
            是身體一整天下來，包括基礎代謝、活動量、吃東西所消耗的熱量。不同的生活型態需要的熱量也不一樣，當每天攝取的熱量和
            TDEE 相等，便達到「熱量平衡」
          </p>
        </div>
        <section class="bmr-box">
          <div class="bmr-item">
            <div class="bmr-img">
              <img src="https://via.placeholder.com/80x80" alt="沒什麼運動量" />
            </div>
            <div class="bmr-body">
              <div class="bmr-txt">沒什麼運動量（幾乎不運動）</div>
              <div class="bmr-count">BMR x 1.2 = <b>1542</b></div>
            </div>
          </div>
          <div class="bmr-item">
            <div class="bmr-img">
              <img src="https://via.placeholder.com/80x80" alt="輕量活動量" />
            </div>
            <div class="bmr-body">
              <div class="bmr-txt">輕量活動量（每週運動 1-3 天）</div>
              <div class="bmr-count">BMR x 1.375 = <b>1766.88</b></div>
            </div>
          </div>
          <div class="bmr-item">
            <div class="bmr-img">
              <img src="https://via.placeholder.com/80x80" alt="中度活動量" />
            </div>
            <div class="bmr-body">
              <div class="bmr-txt">中度活動量（每週運動 3-5 天）</div>
              <div class="bmr-count">BMR x 1.55 = <b>1991.75</b></div>
            </div>
          </div>
          <div class="bmr-item">
            <div class="bmr-img">
              <img src="https://via.placeholder.com/80x80" alt="高度活動量" />
            </div>
            <div class="bmr-body">
              <div class="bmr-txt">高度活動量（每週運動 6-7 天）</div>
              <div class="bmr-count">BMR x 1.725 = <b>2210.2</b></div>
            </div>
          </div>
          <div class="bmr-item">
            <div class="bmr-img">
              <img
                src="https://via.placeholder.com/80x80"
                alt="非常高度活動量"
              />
            </div>
            <div class="bmr-body">
              <div class="bmr-txt">非常高度活動量（一天訓練兩次）</div>
              <div class="bmr-count">BMR x 1.9 = <b>2441.5</b></div>
            </div>
          </div>
        </section>
      </div>
      <div class="section section3">
        <div class="count-box">
          <h2 class="count-title">還剩卡路里</h2>
          <table class="count-table">
            <thead>
              <tr>
                <th>目標</th>
                <th></th>
                <th>食品</th>
                <th></th>
                <th>運動</th>
                <th></th>
                <th>剩餘</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>1766.88</td>
                <td>-</td>
                <td>766</td>
                <td>+</td>
                <td>20</td>
                <td>=</td>
                <td>1020.88</td>
              </tr>
            </tbody>
          </table>
        </div>
        <div class="input-box">
          <select name="meal" id="meal-select">
            <option value="breakfast">早餐</option>
            <option value="lunch">午餐</option>
            <option value="dinner">晚餐</option>
            <option value="snack">點心/下午茶</option>
          </select>
          <input type="text" placeholder="輸入餐點名稱" />
          <input type="number" placeholder="輸入卡路里" />
          <button>新增</button>
        </div>
        <div class="meal-box">
          <table>
            <tr>
              <td>早餐</td>
              <td>麵包</td>
              <td>300大卡</td>
            </tr>
            <tr>
              <td>午餐</td>
              <td>蔬菜沙拉</td>
              <td>150大卡</td>
            </tr>
            <tr>
              <td>晚餐</td>
              <td>燉牛肉</td>
              <td>500大卡</td>
            </tr>
            <tr>
              <td>點心/下午茶</td>
              <td>水果沙拉</td>
              <td>100大卡</td>
            </tr>
            <tr>
              <td>晚餐</td>
              <td>炒麵</td>
              <td>450大卡</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>
