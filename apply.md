CREATE TABLE `apply` (
  `apply_id` int NOT NULL AUTO_INCREMENT COMMENT 'PK',
  `bld_nm` varchar(400) DEFAULT NULL COMMENT '건축물명',
  `bld_kind` varchar(10) DEFAULT NULL COMMENT '공공/민간 선택',
  `bld_corpid` varchar(13) DEFAULT NULL COMMENT '법인등록번호',
  `bld_rep` varchar(20) DEFAULT NULL COMMENT '대표자',
  `bld_date` varchar(14) DEFAULT NULL COMMENT '준공일 yyyyMMddHHmmss',
  `bld_addr` varchar(140) DEFAULT NULL COMMENT '소재지 주소',
  `apply_date` varchar(14) DEFAULT NULL COMMENT '신청일자 yyyyMMddHHmmss',
  `apply_applicant` varchar(20) DEFAULT NULL COMMENT '신청인',
  `apply_agent` varchar(20) DEFAULT NULL COMMENT '(또는 대리인)',
  `apply_privacy` tinyint DEFAULT NULL COMMENT '상태: 0=거부 / 1=동의',
  `apply_terms` tinyint DEFAULT NULL COMMENT '상태: 0=거부 / 1=동의',
  `apply_status` tinyint DEFAULT '0' COMMENT '상태: 0=신청 / 1=거부 / 2=보류 / 3=승인',
  `created_at` varchar(14) DEFAULT NULL,
  PRIMARY KEY (`apply_id`)
) ENGINE=InnoDB AUTO_INCREMENT=7 DEFAULT CHARSET=utf8mb3
