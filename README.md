const Timetable = require('comcigan-parser');
const timetable = new Timetable();

const test = async () => {
  await timetable.init();

  // 학교 검색 및 특정 학교 찾기
  const schoolList = await timetable.search('인주중학교');
  console.log(schoolList);
};

test();
