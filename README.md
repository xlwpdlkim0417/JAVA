CREATE TABLE `apply_member` (
  `apply_mem_id` int NOT NULL AUTO_INCREMENT COMMENT 'PK',
  `apply_id` int DEFAULT NULL COMMENT 'apply_id.apply (FK)',
  `mem_name` varchar(20) DEFAULT NULL COMMENT '성명',
  `mem_officeph` varchar(14) DEFAULT NULL COMMENT '전화 번호(사무실)',
  `phone` varchar(14) DEFAULT NULL COMMENT '휴대폰번호',
  `mem_company` varchar(50) DEFAULT NULL COMMENT '회사명(부서명)',
  `mem_position` varchar(50) DEFAULT NULL COMMENT '직위',
  `mem_email` varchar(50) DEFAULT NULL COMMENT '전자우편',
  `role` tinyint DEFAULT NULL COMMENT '관리자종류: 1 = 총괄매니저 / 2 = 현장관리자',
  `created_at` varchar(14) DEFAULT NULL,
  `mem_id` int DEFAULT NULL,
  PRIMARY KEY (`apply_mem_id`)
) ENGINE=InnoDB AUTO_INCREMENT=17 DEFAULT CHARSET=utf8mb3
