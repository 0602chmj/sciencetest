from pathlib import Path
p = Path("/mnt/data/daegu_science_practice_app.html")
html = p.read_text(encoding="utf-8")

html = html.replace(
'<p>객관식 5문제와 서술형 5문제, 총 10문제입니다. 답을 제출하면 점수와 해설을 확인할 수 있어요.</p>',
'<p>객관식 5문제와 서술형·창의탐구 5문제, 총 10문제입니다. 다시 시작할 때마다 문제 은행에서 새로운 조합을 뽑아요.</p>'
)
html = html.replace(
'<p class="small">서술형은 핵심 개념과 과학적 근거를 기준으로 간단 채점합니다. 다양한 정답 표현이 있을 수 있으니 해설도 꼭 확인하세요.</p>',
'<p class="small">서술형은 핵심 개념어가 포함되면 표현이 달라도 점수를 인정합니다. 창의·탐구 문제는 NASA의 공개 과학·공학 활동을 참고해 만들었으며, 정답이 하나로 정해지지 않는 문제입니다.</p>'
)

start = html.index("const questions=[")
end = html.index("let answers=", start)

js = r'''const questionBank=[
{type:"객관식",q:"질량이 다른 두 물체를 같은 높이에서 놓는다. 공기 저항이 없을 때 바닥에 도착하는 순간 두 물체의 속력은?",opts:["무거운 물체가 더 빠르다","가벼운 물체가 더 빠르다","두 물체의 속력은 같다","질량만으로는 비교할 수 없다"],a:2,why:"공기 저항이 없고 같은 높이에서 정지 상태로 출발하면 질량과 관계없이 도착 속력은 같습니다."},
{type:"객관식",q:"모래와 물이 섞인 혼합물에서 모래를 분리하는 가장 알맞은 방법은?",opts:["증발","거름","증류","자석 이용"],a:1,why:"거름은 액체는 통과시키고 물에 녹지 않는 고체를 걸러 냅니다."},
{type:"객관식",q:"식물의 광합성이 주로 일어나는 곳은?",opts:["뿌리","꽃잎","잎","씨앗"],a:2,why:"잎의 엽록체에서 빛에너지를 이용해 광합성이 주로 일어납니다."},
{type:"객관식",q:"낮과 밤이 생기는 가장 직접적인 원인은?",opts:["지구의 자전","지구의 공전","달의 자전","태양의 움직임"],a:0,why:"지구가 자전하면서 태양을 향한 쪽은 낮, 반대쪽은 밤이 됩니다."},
{type:"객관식",q:"태양광 패널의 각도에 따른 발전량을 비교하려 한다. 공정한 실험 방법은?",opts:["패널 각도와 빛의 세기를 동시에 바꾼다","패널 각도만 바꾸고 나머지 조건은 같게 한다","측정 시간을 매번 다르게 한다","패널 크기를 매번 바꾼다"],a:1,why:"한 번에 한 조건만 바꾸고 빛의 세기, 패널 종류, 측정 시간 등은 같게 해야 합니다."},
{type:"객관식",q:"물에 소금을 녹인 소금물에서 소금을 얻으려면 가장 알맞은 방법은?",opts:["거름","자석","증발","체로 거르기"],a:2,why:"물을 증발시키면 물은 기체가 되어 빠져나가고 소금이 남습니다."},
{type:"객관식",q:"전구 두 개를 한 회로에 직렬로 연결했을 때 한 전구를 빼면 일반적으로 어떻게 될까?",opts:["다른 전구가 더 밝아진다","다른 전구도 꺼진다","다른 전구 밝기는 그대로다","전지가 더 강해진다"],a:1,why:"직렬회로는 전류가 흐르는 길이 하나이므로 한 곳이 끊기면 회로 전체에 전류가 흐르지 않습니다."},
{type:"객관식",q:"소리가 전달되기 위해 반드시 필요한 것은?",opts:["빛","물질로 된 매질","진공","햇빛"],a:1,why:"소리는 물질의 진동으로 전달되므로 진공에서는 전달되지 않습니다."},
{type:"객관식",q:"얼음이 녹는 동안 온도가 한동안 거의 일정한 까닭은?",opts:["열을 전혀 받지 않아서","받은 열이 상태 변화에 쓰여서","얼음의 질량이 사라져서","주변 공기가 차가워져서"],a:1,why:"녹는점에서 공급된 열은 온도를 높이기보다 고체에서 액체로 상태를 바꾸는 데 쓰입니다."},
{type:"객관식",q:"같은 크기의 힘으로 물체를 밀 때 바닥의 마찰력이 작아지면 물체의 운동은 어떻게 되기 쉬울까?",opts:["움직이기 더 어려워진다","더 쉽게 움직인다","질량이 사라진다","중력이 없어진다"],a:1,why:"마찰력이 작아지면 운동을 방해하는 힘이 줄어 물체를 더 쉽게 움직일 수 있습니다."},

{type:"서술형",q:"따뜻한 물에서 설탕이 더 빨리 녹는 까닭을 입자 운동과 연결해 설명해 보세요.",groups:[["온도","따뜻"],["입자"],["운동","활발"],["빨리","속도"]],sample:"물의 온도가 높으면 물 입자의 운동이 활발해져 설탕이 더 빠르게 녹을 수 있다.",why:"온도가 높아지면 입자 운동이 활발해져 용해 속도가 빨라질 수 있습니다."},
{type:"서술형",q:"식물에 주는 물의 양이 성장에 미치는 영향을 알아보려 합니다. 바꾸는 조건과 같게 해야 할 조건을 각각 써 보세요.",groups:[["물의 양","물 양"],["빛","햇빛"],["종류","식물"],["흙","온도","화분"]],sample:"물의 양만 바꾸고 식물의 종류, 햇빛의 양, 흙과 화분은 같게 한다.",why:"한 번에 한 조건만 바꾸고 다른 조건은 같게 해야 물의 양의 영향을 비교할 수 있습니다."},
{type:"서술형",q:"태양광 패널로 선풍기를 작동시킬 때 에너지가 바뀌는 순서를 설명해 보세요.",groups:[["빛","태양"],["전기"],["운동","회전"]],sample:"빛에너지가 전기에너지로 바뀌고, 모터에서 운동에너지로 바뀐다.",why:"핵심 흐름은 빛에너지 → 전기에너지 → 운동에너지입니다."},
{type:"서술형",q:"교실에서 전기를 아끼는 자동 장치를 제안하고, 작동 원리를 설명해 보세요.",groups:[["센서","감지"],["사람","움직임"],["자동"],["끄","꺼"]],sample:"사람 감지 센서가 교실에 사람이 없음을 확인하면 조명을 자동으로 끈다.",why:"사람이나 밝기를 감지해 필요한 때만 전기를 사용하면 낭비를 줄일 수 있습니다."},
{type:"서술형",q:"숲의 나무가 많이 사라지면 생태계와 주변 환경에 생길 수 있는 변화 두 가지와 해결 방법을 써 보세요.",groups:[["서식지","동물"],["토양","흙","침식"],["이산화탄소","탄소","온실"],["나무","심","산불","보호"]],sample:"동물의 서식지가 줄고 토양 침식이 커질 수 있다. 나무를 심고 숲을 보호한다.",why:"나무는 동물의 서식지를 제공하고 토양을 붙잡으며 이산화탄소를 흡수합니다."},
{type:"서술형",q:"얼음이 물에 뜨는 현상을 밀도라는 말을 사용해 설명해 보세요.",groups:[["얼음"],["밀도"],["물보다","작"],["뜬","뜨"]],sample:"얼음은 물보다 밀도가 작기 때문에 물에 뜬다.",why:"같은 부피를 비교하면 얼음의 질량이 물보다 작아 밀도가 낮습니다."},
{type:"서술형",q:"전구 두 개를 직렬로 연결한 회로와 병렬로 연결한 회로의 차이를 한 가지 설명해 보세요.",groups:[["직렬"],["병렬"],["전류","길","경로"]],sample:"직렬은 전류가 흐르는 길이 하나이고, 병렬은 전류가 흐르는 길이 여러 갈래다.",why:"직렬은 하나의 경로를 공유하고 병렬은 여러 갈래로 나뉩니다."},

{type:"창의·탐구",q:"NASA의 태양광 펌프 설계 활동을 참고한 문제입니다. 햇빛이 약한 날에도 물을 공급하려면 어떤 장치를 더하면 좋을까요? 에너지 저장 또는 물 저장 방법을 포함해 설계해 보세요.",groups:[["배터리","축전","저장"],["물탱크","저수","물 저장"],["태양광","태양"],["펌프","모터","전기"]],sample:"햇빛이 강할 때 태양광 전기로 배터리에 에너지를 저장하거나 물탱크에 물을 미리 저장해 흐린 날 사용한다.",why:"정답은 하나가 아닙니다. 에너지를 저장하거나 물을 미리 저장하는 등 설계의 원리와 장단점을 설명하면 됩니다.",source:"NASA Glenn Engineering Design Challenges",url:"https://www.nasa.gov/stem-content/engineering-design-challenges-from-nasas-glenn-research-center/"},
{type:"창의·탐구",q:"화성 탐사 로봇이 울퉁불퉁한 땅을 지나야 합니다. 바퀴가 빠지거나 넘어지는 일을 줄이려면 바퀴나 로봇의 모양을 어떻게 바꾸면 좋을까요? 이유도 설명해 보세요.",groups:[["바퀴","넓"],["무게중심","중심","낮"],["접지","마찰","미끄럼"],["안정","넘어"]],sample:"바퀴를 넓게 하거나 무게중심을 낮추면 땅에 닿는 면적과 안정성이 커져 덜 빠지고 덜 넘어질 수 있다.",why:"바퀴 폭, 표면 무늬, 무게중심 등 여러 설계가 가능합니다. 어떤 구조가 어떤 문제를 줄이는지 설명하세요.",source:"NASA Glenn Engineering Design Challenges",url:"https://www.nasa.gov/stem-content/engineering-design-challenges-from-nasas-glenn-research-center/"},
{type:"창의·탐구",q:"재난 지역에서 구조 로봇이 사람을 찾는다고 생각해 봅시다. 어둡고 장애물이 많은 곳에서 사람을 안전하게 찾으려면 어떤 센서 두 가지를 사용하고, 각각 어떤 역할을 맡기겠습니까?",groups:[["거리","장애물"],["카메라","열","적외선","온도"],["센서"],["안전","충돌","사람","구조"]],sample:"거리 센서로 장애물을 피하고 카메라나 열 센서로 사람의 위치를 찾는다.",why:"센서마다 측정하는 정보가 다릅니다. 두 센서의 역할을 구분하고 안전과 연결하면 됩니다.",source:"NASA Robotic Search and Rescue Challenge",url:"https://www.nasa.gov/stem-content/robotic-search-and-rescue-challenge/"},
{type:"창의·탐구",q:"달 기지에서 물을 아껴야 합니다. 손을 씻거나 식물을 기르는 데 사용한 물을 다시 활용하는 장치를 설계한다면 어떤 단계로 물을 깨끗하게 만들겠습니까?",groups:[["거름","필터"],["침전","가라앉"],["살균","소독","끓"],["재사용","다시"]],sample:"큰 찌꺼기를 거르고 침전시킨 뒤 필터와 살균 과정을 거쳐 용도에 맞게 재사용한다.",why:"여러 단계의 정화 방법을 제안할 수 있습니다. 정화 후에도 마실 수 있는 물인지 별도로 확인해야 한다는 점을 기억하세요.",source:"NASA STEM learning resources",url:"https://www.nasa.gov/learning-resources/nasa-stem-opportunities-activities/"},
{type:"창의·탐구",q:"학교 운동장에 그늘을 늘리면서 전기도 만들고 싶습니다. 나무를 베지 않는 방법으로 태양광을 설치할 장소와 구조를 제안하고 장점을 설명해 보세요.",groups:[["주차장","통로","운동장","지붕","그늘막"],["태양광","패널"],["그늘","햇빛"],["나무","보호","환경"]],sample:"주차장이나 통로 위에 태양광 지붕을 설치하면 그늘을 만들고 전기도 생산하며 나무를 보존할 수 있다.",why:"설치 장소, 발전 원리, 사람이나 자연에 주는 이점을 연결하면 됩니다.",source:"NASA Engineering in the Classroom",url:"https://www.nasa.gov/stem-content/engineering-in-the-classroom/"},
{type:"창의·탐구",q:"종이컵과 실, 작은 추를 이용해 물체를 목표 지점에 정확히 떨어뜨리는 장치를 만든다고 합시다. 실패했을 때 어떤 조건을 바꾸어 실험하고, 결과를 어떻게 비교하겠습니까?",groups:[["길이","실"],["각도","높이","위치"],["한 가지","하나","조건"],["기록","측정","비교"]],sample:"실의 길이나 출발 높이 중 한 가지를 바꾸고 나머지는 같게 한 뒤 목표 지점에서 얼마나 벗어났는지 기록해 비교한다.",why:"NASA JPL의 공학 활동처럼 설계하고 시험한 뒤 결과를 바탕으로 개선하는 과정이 중요합니다.",source:"NASA JPL On Target",url:"https://www.jpl.nasa.gov/edu/resources/lesson-plan/on-target/"}
];

function pickRandom(arr,n){
 const copy=[...arr];
 for(let i=copy.length-1;i>0;i--){const j=Math.floor(Math.random()*(i+1));[copy[i],copy[j]]=[copy[j],copy[i]]}
 return copy.slice(0,n);
}
function makeQuiz(){
 const mc=pickRandom(questionBank.filter(q=>q.type==="객관식"),5);
 const written=pickRandom(questionBank.filter(q=>q.type!=="객관식"),5);
 return [...mc,...written];
}
let questions=makeQuiz();
'''
html = html[:start] + js + html[end:]

# Replace the keyword matching code with group-based flexible scoring
old = '''   const answer=String(answers[i]||"").trim();const hits=q.keywords.filter(k=>answer.includes(k)).length;
   earned=answer.length?Math.min(10,Math.round(hits/q.keywords.length*10)):0;
   detail=`내 답: ${answer?escapeHtml(answer):"미응답"}<br>참고 답안: ${q.sample}<br><span class="small">핵심어 ${hits}/${q.keywords.length}개 포함 기준의 참고 점수입니다. 표현이 달라도 과학적으로 맞으면 정답일 수 있어요.</span>`;'''
new = '''   const answer=String(answers[i]||"").trim();
   const groups=q.groups||[];
   const hits=groups.filter(group=>group.some(word=>answer.toLowerCase().includes(word.toLowerCase()))).length;
   earned=answer.length?Math.round(hits/Math.max(groups.length,1)*10):0;
   if(answer.length && hits===groups.length) earned=10;
   detail=`내 답: ${answer?escapeHtml(answer):"미응답"}<br>참고 답안: ${q.sample}<br><span class="small">핵심 개념 ${hits}/${groups.length}개 확인 · 같은 뜻의 핵심어 중 하나만 들어 있어도 인정합니다. 핵심 개념이 모두 포함되면 만점입니다.</span>`;'''
if old not in html:
    raise ValueError("old scoring block not found")
html = html.replace(old, new)

# Include source links on creative questions' explanations
old2 = '''  reviews+=`<div class="review"><b>${i+1}번 · ${q.type}</b> <span class="${earned>=7?"correct":"wrong"}">${earned}/10점</span><p>${detail}</p><p><b>해설:</b> ${q.why}</p></div>`;'''
new2 = '''  const sourceLink=q.url?`<p class="small">참고한 인터넷 자료: <a href="${q.url}" target="_blank" rel="noopener">${escapeHtml(q.source)}</a></p>`:"";
  reviews+=`<div class="review"><b>${i+1}번 · ${q.type}</b> <span class="${earned>=7?"correct":"wrong"}">${earned}/10점</span><p>${detail}</p><p><b>해설:</b> ${q.why}</p>${sourceLink}</div>`;'''
if old2 not in html:
    raise ValueError("review block not found")
html = html.replace(old2, new2)

# Fresh randomized quiz every time the user retries
html = html.replace(
'$("again").onclick=()=>{answers=Array(questions.length).fill(null);idx=0;$("result").classList.add("hidden");$("quiz").classList.remove("hidden");showQuestion();window.scrollTo(0,0)};',
'$("again").onclick=()=>{questions=makeQuiz();answers=Array(questions.length).fill(null);idx=0;$("result").classList.add("hidden");$("quiz").classList.remove("hidden");showQuestion();window.scrollTo(0,0)};'
)

# Better notice and total description
html = html.replace(
'안내: 이 앱의 문항은 학습용으로 새로 만든 <b>창작 연습문제</b>입니다. 실제 기출문제나 대구교대의 공식 출제문제가 아닙니다.',
'안내: 객관식·서술형은 학습용으로 새로 만든 연습문제입니다. 창의·탐구 문항은 NASA의 공개 교육 자료와 공학 활동을 참고해 구성했습니다. 실제 기출문제나 대구교대의 공식 출제문제는 아닙니다.'
)

p.write_text(html, encoding="utf-8")
print(f"수정 완료: {p} ({p.stat().st_size:,} bytes)")
